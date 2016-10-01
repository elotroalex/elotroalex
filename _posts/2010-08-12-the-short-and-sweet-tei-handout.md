---
title: The short-and-sweet TEI handout
author: elotroalex
layout: post
permalink: /the-short-and-sweet-tei-handout/
btc_comment_counts:
  - 'a:0:{}'
btcnew_post:
  - 'a:6:{s:2:"ID";s:2:"44";s:13:"post_date_gmt";s:19:"2010-08-12 20:35:25";s:23:"initial_import_date_gmt";s:19:"2011-02-22 00:31:56";s:20:"last_import_date_gmt";s:19:"2011-02-22 00:31:56";s:4:"hits";s:1:"0";s:6:"misses";s:1:"1";}'
btcnew_comment_counts:
  - 'a:0:{}'
btcnew_comment_summary:
  - 'a:0:{}'
categories:
  - Digital Humanities
---
</p> </p> 

For the past few weeks, I’ve been working with some colleagues to develop a model for incorporating the full digitization of a scholarly work into a literature course. The process goes from scanning to OCR to tagging. The goal is for students to learn some of the basics of digital humanities while producing image-text PDFs and TEI-lite versions of works that might be publishable online in the future. Below is a sample of the student handout. This version of the handout is meant for the tagging of a 200-300 page scholarly work to be done by a team of 4-5 students. You can download and use a full version of the handout <a href="https://docs.google.com/document/edit?id=12ErwXGHGaFL71M3cWHpI6gkfVzzsKHfk7U6N6vRmIS4&authkey=CKG3l6oG&hl=en#" target="_blank">here</a>. In the next few weeks, I will be working on developing a similar model meant for primary texts, so stay tuned.

## &#160;

> ## XML and books
> 
> XML stands for EXtensible Markup Language and as the word markup implies, it is a tool used to describe data. HTML, which you may be more familiar with, shares many similarities with XML, most importantly the use of *tags *< >. The “data” in HTML consists of instructions for browsers; in XML, on the other hand, there is no predefined use or vocabulary for the tags (hence the “EXtensible” in XML). For example, if you own a pink Chihuahua named Pepe, you could “express” it in XML this way:
> 
> `
<p><dog type=”mine” name=”pepe”></p>
<p style="text-indent: 25px"><color>pink</color></p>
<p style="text-indent: 25px"><breed>Chihuahua</breed></p>
<p></dog></p>
<p>`  
> 
> 
> <table border="1" cellspacing="0" cellpadding="5" width="490">
>   <tr>
>     <td valign="top" width="498">
>       <p>
>         <b>TIP:</b> For a longer introduction to XML, visit <a href="http://www.w3schools.com/xml/default.asp">w3Schools</a>.
>       </p>
>     </td>
>   </tr>
> </table>
> 
> In a sense, all texts can be said to contain data of a certain kind. Literature and criticism are no exception to this rule. XML helps you name and organize that data. With XML, the possibilities are legion: we could, for example, name the kinds of content we find (<metaphor>, <character>, etc.), describe the physical attributes of a book (<paper>, <ink>, etc.), how a text is laid out (<column>, <page_break>, etc.) or the logical units of a text (<line>, <paragraph>, etc).
> 
> Because there are so many possibilities, scholars and scientists all over the world have agreed to use standards in their fields. In digital humanities, the most important standard set of predetermined tags, or *tag-set,* is the one provided by the Text Encoding Initiative (TEI). In this class we will be using an even smaller subset of that standard called TEI-lite to introduce you to the practice of *tagging*.
> 
> <table border="1" cellspacing="0" cellpadding="5" width="490">
>   <tr>
>     <td valign="top" width="498">
>       <p>
>         <b>TIP:</b> To deepen your knowledge of TEI and TEI-lite, you can explore <a href="http://www.google.com/url?q=http%3A%2F%2Ftbe.kantl.be%2FTBE%2FTBE.htm&sa=D&sntz=1&usg=AFQjCNGDPlYNKAfenkEpinrS8FlJRZkKUg">TEI by example</a> or read the <a href="http://www.tei-c.org/Guidelines/Customization/Lite/">TEI-lite documentation</a>.
>       </p>
>     </td>
>   </tr>
> </table>
> 
> A basic TEI file includes a text (the linguistic content) and *meta-data *(information about the text). The first three tags you will learn already express the basic structure of a TEI file. The topmost tag includes all other tags and is named <TEI>. The tag which includes the information about the text is called the <teiHeader> and always precedes the tag which includes the text, appropriately named <text>.
> 
> The overall structure of the TEI file then looks something like this:
> 
> `
<p><TEI></p>
<p style="text-indent: 25px"><teiHeader></p>
<p style="text-indent: 50px">[information about the text]</p>
<p style="text-indent: 25px"></teiHeader></p>
<p style="text-indent: 25px"><text></p>
<p style="text-indent: 50px">[the text itself]</p>
<p style="text-indent: 25px"></text></p>
<p></TEI></p>
<p>`</blockquote>