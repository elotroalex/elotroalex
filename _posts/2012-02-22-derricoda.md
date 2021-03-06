---
title: Derri(co)da
author: elotroalex
layout: post
permalink: /derricoda/
categories:
  - Digital Humanities
---
<p>
  [A slightly modified version of this post was originally posted as a <em>code-critique</em> for the <a title="CCS2012" href="http://haccslab.com/?page_id=174" target="_blank">Critical Code Studies Working Group 2012</a>]
</p>



<p>
  Prior to anything else, I wanted to thank the organizers for inviting me and inspiring such an engaging debate.
</p>

<p>
  I apologize for my late entry. Except for a premature comment on week 2, I have been just observing and absorbing, never sure when was the right time to join the dance. My hesitation comes as much from a noob-complex as from the nature of my intervention. In brief, I want to explore the ways in which critical discourse in general and literary criticism in particular are already procedural, and what it would mean to write code to express and critique natural language discourse. The can of worms I feel I am opening has been opened before in many different contexts, going as far back as Aristotle in my estimation. We could justify my intervention by claiming that any code we could generate to express or critique natural language discourse can itself be critiqued back from a CCS point of view. The process looks something like this:
</p>

<p>
</p>

<p>
  <blockquote>
    <p>
      Human Discourse—> Analogical Code—> Code Critique
    </p>
  </blockquote>
  
  <p>
    The example texts that I want to use themselves generate a further mirroring that might throw this half-blind enterprise into the proverbial <em>mise-en-abyme</em>. We play at <a href="http://www.imdb.com/title/tt0089881/">the edge of the cliff</a> at our own pleasure! The example texts have been collected under the title, <em>Ulysse gramophone/Deux mots pour Joyce</em> by Jacques Derrida, and published by Éditions Galilée in 1987. If I am not mistaken, the texts are available in translation in Derek Attridge&#8217;s compilation <em><a href="http://books.google.com/books/about/Acts_of_literature.html?id=W7eLlRE-5OwC">Acts of Literature</a></em>. As far as I know, they are the first sustained attack by Derrida on what was then (1980s) called humanities computing, though that attack was an extension of his life-long agonism with formal logic. It also happens to be the first time Derrida engages with Joyce directly. In these studies, both originally delivered as talks, Derrida makes several moves that made him an irresistible target for my meditations on discourse and procedure.
  </p>

<p>
  Let me start by making the most dangerous move and offer a brief of Derrida&#8217;s relevant points for those who are not familiar with these texts:
</p>


<ul>
    <li>
      <span style="font-family: Arial, Verdana;">Derrida claims that Joyce is a &#8220;<em>logiciel</em>&#8221; (~software), a &#8220;<em>joyciciel</em>&#8221; (22-23) that reduces our computers to &#8220;<em>un jouet d&#8217;enfant préhistorique</em>&#8221; (a prehistorical child&#8217;s toy). Granted, he made his claims before the advent of the internet, but his comments were mostly directed at the <em>logic</em> part of <em>logiciel,</em> so <em>&#8230;</em></span>
    </li>
    <li>
      <span style="font-family: Arial, Verdana;">According to Derrida, the main power of the <em>joiciciel</em> lies in its ability to predict the scholarly moves of generations of Joyce scholars to come.</span>
    </li>
    <li>
      <span style="font-family: Arial, Verdana;">Derrida claims that we cannot exhaust the identities held <em>in potentia</em> by the portmanteaus and puns in Joyce, nor can we reduce any word deployed by Joyce to an identity in the first place. To prove his point he uses the lines &#8220;He War&#8221; from <em>Finnegans Wake</em> (FW) in <em>Deux mots pour Joyce</em> (DMPJ) and the word &#8220;Yes&#8221; from <em>Ulysses</em> (U) in <em>Ulysse gramophone</em> (UG). Notice for example how &#8220;He War&#8221; could point to many different languages to generate &#8220;He was,&#8221; &#8220;He was war,&#8221; &#8220;He who was is war,&#8221; plus it suggests many homophones &#8220;hear,&#8221; &#8220;ar,&#8221; &#8220;ear,&#8221; usw. In the case of &#8220;Yes&#8221; Derrida points us to the many different contexts, as he is wont to do, to show how unstable that little word can be. My favorite one is the example of the &#8220;<em>Oui</em>?&#8221; that the French use when they answer the phone to say our &#8220;Hello&#8221; or as Derrida would have it, &#8220;<a href="http://en.wikipedia.org/wiki/Interpellation_(philosophy)">Yes, I am here</a>.&#8221; </span>
    </li>
    <li>
      <span style="font-family: Arial, Verdana;">Finally, Derrida claims that the whole of the academic enterprise is itself a &#8220;computer <em>de toute la memoire</em>&#8221; (a computer of all memory), whose main goal has been to &#8220;<em>programmer pendant des siècles la totalité des recherches dans le champ onto-logico-encyclopédique &#8212; tout en commémorant sa propre signature</em>,&#8221; (to program for centuries the totality of research in the onto-logico-encyclopedic field &#8212; all the while celebrating its own signature) (97). In this regard, he contends that experts are &#8220;pre-programmed&#8221; by their research questions, especially by those limits we impose on what counts as a valid intervention or not. Funny, that he reduces others to procedural approaches while sparing himself and Joyce!</span>
    </li>

  </ul>
  
  <p>
    As you can see, this is begging to be addressed. I feel like I can probably write pages of critical prose in response, but I thought that a more appropriate response would be in the form of what I call &#8216;useless&#8217; code, one that exploits the &#8220;extra-functional significance,&#8221; that many of you wish to derive from perfectly useful code. This whim is both a goad to push me to deepen my code &#8216;competency,&#8217; as @samplereality would have it, and the cheekiest revenge on such a Gargantuan critique of computational methods. Consider this also to be my call for a more able <em>procedularist</em> to help me answer Derrida&#8217;s (and apparently Joyce&#8217;s) challenge.
  </p>
  
  
  <p>
    Here is one of the tentative avenues by which I think we can approach this hydra, brought to you in an appropriately unnecessary:
  </p>



<p>
    <strong>We can attempt to code Derrida&#8217;s own scholarly methods:</strong><br /> He begins his study of the word &#8220;yes&#8221; in Ulysses by counting 222 occurrences&#8230; by hand. (74) He immediately follows with a playful footnote where he quotes another scholar citing 354 occurrences. Counting words is trivial, and Derrida only does so to complicate it immediately by pointing out that the other scholar also noted that the Irish &#8216;ay&#8217; should be counted as well. Derrida will then spend countless pages showing how a) &#8216;yes&#8217; can be said without saying it and by other means (including the word &#8216;no&#8217;!); and, b) that saying &#8216;yes&#8217; itself says many different things. The point is, of course, that we can never exhaust the possibilities computationally. It is here that we agree with Derrida, but rewrite his &#8216;proof&#8217; using useless code, one rhetorical move at a time. Take for example the following line from Derrida: &#8220;<em>Yes ne peut donc être, dans</em> Ulysse,<em> qu&#8217;une marque à la fois parlée et écrite, vocalisée comme graphème et écrite comme phonème, oui, en un mot</em> gramophoné&#8221; (Yes has no other choice but to be, in Ulysses, both spoken and written, vocalized as grapheme and written as phoneme—yes, in a word, gramophoned) (75). Well here&#8217;s a (naive) tiny code-critique:</span></span></p> 

    Required: <a href="http://www.speech.cs.cmu.edu/cgi-bin/cmudict">CMUdict</a>
    <br /> Language: pseudo-Ruby<br /> 
</p>

~~~ ruby

Class Word
  def tokenize_written
    # tokenize words in your fave edition of Ulysses
  end 

  def tokenize_spoken
    #load up the CMUdict or equiv.
  end 

  def find_match
    # initialize tokenize_written and tokenize_spoken
    # find possible matches between words and phonemic
    # transliterations
  end 

  derrida_yes = Word.new (&#8216;yes&#8217;)
  if derrida_yes.find_match == true
    puts="Derrida was right after all!"
  else
    puts="Bunk!"
  end
~~~
        
<p>
  <span style="font-family: Arial, Verdana;">I close by inviting you to think of other ways in which we can use code to re-express critical discourse and in which procedural thinking can be used as an analogy for specific rhetorical/scholarly gestures. Could it be useful, say to re-write by other means the history of criticism? Am I wrong, or just wrong-headed?</span>
</p>