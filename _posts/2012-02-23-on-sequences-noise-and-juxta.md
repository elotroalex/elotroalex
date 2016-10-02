---
title: on sequences, noise and Juxta.
author: elotroalex
layout: post
permalink: /on-sequences-noise-and-juxta/
btcnew_comment_summary:
  - 'a:0:{}'
btcnew_post:
  - 'a:6:{s:2:"ID";s:3:"878";s:13:"post_date_gmt";s:19:"2012-02-23 04:44:32";s:23:"initial_import_date_gmt";s:19:"2012-02-23 04:46:41";s:20:"last_import_date_gmt";s:19:"0000-00-00 00:00:00";s:4:"hits";s:1:"0";s:6:"misses";s:1:"0";}'
btcnew_comment_counts:
  - 'a:0:{}'
categories:
  - Césaire
  - Digital Humanities
---
[Cross-posted at <a href="http://www.nines.org/news/?p=1523" target="_blank">the NINES blog</a>]

If you mention tokens and strings to a textual scholar, do not be surprised to receive a polite reprimand in response. Most consider the vocabulary inherited from computer science undeserving of the rich realities of the texts they hold hear, and with good reason. We have already endured an uphill battle against older, more insidious forms of abstraction that would have us believe texts are written in the heavens with capital T&#8217;s. At the same time, a growing number of well intentioned scholars are content to use digital tools that manipulate texts precisely at this level, without asking too many impertinent questions about the black-box processes that give them handy results. The classic example of this disavowal is the black-boxed use of Google, which I venture has become a staple of scholarship everywhere. In a sense, we are all forced in one way or another to rely on black-boxing. Slowly but surely, we realize we are in a world of &#8220;[black-boxes all the way down][1].&#8221;

Despite the need to black-box some areas of our workflow in order to move along, we ignore some black-boxes at our own peril. Not only do we risk transferring agency to a half-understood process, we may miss key insights on our own scholarly procedures. After a few years of using the Juxta tool to help me collate the fascinating mutations of Aimé Césaire&#8217;s *Et les chiens se taisaient*, I finally took a peek inside the internal processes of the software. In my defense, I really wasn&#8217;t ready to look behind the curtain before dusting off my math skills, learning some of the basic vocabulary of computer science and acquiring basic code literacy. Although I still feel there is much more to understand, I have seen enough to know that I can never look at comparisons or textuality the same way again.

Perhaps a bit of background would be in order. As I pointed out in [an earlier post][2], Juxta cannot handle the Césaire texts adequately unless you break them into smaller chunks. The main problem was and is the large amount of transpositions between one version and the next of *Et les chiens se taisaient*. I did the work of cataloguing and diagramming the many &#8216;moves&#8217; by hand, using Juxta to compare each block of text internally. Earlier this year I started having doubts about my ability to capture all matching blocks between one version and the next, especially those comparisons that revealed upwards of 70 moves! I noticed that Juxta caught *some* matches, so I tried a small experiment.

I took my working text of the typescript (TS) and the *editio princeps* (EP) and processed them whole through Juxta. I carefully used the results to remove from the original TS and EP files all the matches caught by the first run. Once I had removed every match from both files, I ran those smaller files. Of course, the next set of matches was different than the first. I went ahead and carefully removed those matches from the files. This process continued for 10 or 11 runs, until I eventually had two tiny files with text I was reasonably certain was mutually exclusive. I was so excited, I even made [a screencast][3] explaining the process. (Later I realized that this method does not guarantee 100% accuracy, but I&#8217;m getting ahead of myself).

The experiment proved that I had indeed missed some matches, despite months of working with these texts the traditional way. I was very satisfied with my ingenuity, but I still didn&#8217;t understand why Juxta matched some things and not others. While I was thus occupied, a team of friends and colleagues were beginning to see some positive results porting the output of [SuperFastMatch][4] to the Juxta API. My dream of having my texts represented using the powerful Juxta visualization suite was getting so close I could taste it. But&#8230; I understood even less about SuperFastMatch than I did about diff. Enough was enough.

I had the faint notion that Juxta used a modified version of the <a href="http://en.wikipedia.org/wiki/Diff" target="_blank">diff</a> utility, so I started my research there. Apparently, the diff family builds on a solution to the [longest common subsequence problem][5]. What Juxta was catching as a match in every run of my experiment was indeed a longest common subsequence. Here is where a hundred questions, questions I would&#8217;ve never thought to ask had I stayed outside the box, took center stage in my research: What does it mean that a complex comparison set has several levels of overlapping subsequences? What do these levels tell us about textual sequence in general? What&#8217;s the relationship between these sequences and the process by which a text is actually rearranged from one version to the next by human agency?

String matching 101: The longest common subsequence of any two strings compared to each other is that set of tokens that follow each other in the same linear order in both strings, despite any intervening tokens. In the case of Juxta, which seems to be running a <a title="wdiff" href="http://www.gnu.org/software/wdiff/" target="_blank">wdiff</a> flavor of the <a title="diff-patch-match" href="http://code.google.com/p/google-diff-match-patch/" target="_blank">Google diff tools</a>, the tokens in question are words. For example, given the following two strings, where each token is represented by a letter of the alphabet: 1) ABCXDEYFZ, and 2) ABMCDXYZEFN, the sequence ABCDEF can be said to be the longest common subsequence. If we ran this example through Juxta, M, N, X, Y and Z would be highlighted in green, while the longest common subsequence would remain unformatted. This is the principal method by which Juxta can claim to mark difference. As long as you work with simple texts, texts in which there is one clearly recognizable longest common subsequence with minor interruptions, this technique can be very effective. On the other hand, texts with many transpositions &#8216;break&#8217; because mutually-exclusive large subsequences intersect eachother. Realizing the reason for Juxta&#8217;s limitations, I couldn&#8217;t help but think that textual scholars have also been operating using a human version of the diff, assuming a long stable sequence against which differences move about.

A few weeks ago, I also started thinking about the possibility of automating my experiment by writing a script to do what I was doing &#8216;by hand.&#8217; I baptized my method Poor Man&#8217;s String Matching, but it could more appropriately be called an iterative diff. Once I set out to do the work of recognizing and stashing sequences programmatically, I started seeing the problems with my solution. Though these problems are not insurmountable, they reveal an enormous amount about our assumptions.

The two main problems are handling &#8216;noise&#8217; and defining what counts as a coherent textual block. The latter is too difficult a problem to cover in a blogpost, but it is important enough that I dedicate a chapter of my dissertation, endearingly called &#8220;Legology,&#8221; to solving it. I take *Noise* to be those little isolated fragments, usually single words, that are part of the longest common subsequence, but which cannot be said to belong to a textual block. Here is where the humanist parts way with the computer scientist or the mathematician. For these two, even a value of zero can be counted as a sequence! Although there can be isolated tokens that could interest a scholar comparing two texts (rare words or proper names, for example), we are more often than not going to worry about two or more concatenated words, and we would certainly not call anything less a sequence. At least, I wouldn&#8217;t.

<p>
  Noise can be of two kinds: The noise that happens outside of the blocks of interest, and the noise within blocks of interest. In Juxta these can be seen as white fragments in a sea of green, and green fragments in a sea of white. These are very different creatures and also need to be dealt separately. Noise can lead to small errors if we were to run a straight iterative diff, eliminating every longest common subsequence in each iteration. The errors come from the probability that a word caught in a sequence belongs to a smaller intersecting common subsequence.
</p>

<p>
  To understand this properly, imagine we compare the results of the first diff run to the results of a human being who only matches blocks of text that are clearly matches. The human&#8217;s results would not be exactly the longest common subsequence, but they would definitely be more useful. Since we are interested in blocks, chances are letting the computer net everything would probably lead to the accidental disintegration of smaller blocks of interest.
</p>

<p>
  Just as I learned some odd lessons about the role of sequence in comparison sets by studying the longest common subsequence problem, I also found some unexpected lessons about textuality from trying to solve the noise problem. If you&#8217;re interested in my solution, I invite you to read my dissertation when it comes out. In the meantime, I encourage the textual scholars who are reading this to try to solve these problems on their own, to engage with the procedures that make our machines tick, and to do it without taking off their humanities hats.
</p>

<p>
  If we don&#8217;t learn how to think <em>with</em> our machines, what choice will they have but to think for us?
</p>

 [1]: http://snightingale.tumblr.com/post/15785278074/black-boxes-all-the-way-down
 [2]: http://www.juxtasoftware.org/?p=99
 [3]: http://vimeo.com/34418392
 [4]: https://github.com/mediastandardstrust/superfastmatch
 [5]: http://en.wikipedia.org/wiki/Longest_common_subsequence_problem