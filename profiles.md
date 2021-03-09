---
layout: page
title: Profiles
author: Alex Gil
permalink: /profiles/
---



<h2>Redux</h2>

I am the Digital Scholarship Librarian at Columbia University, where I collaborate with faculty, students and library colleagues in humanities research, pedagogy or knowledge production that involves the use of advanced computation, digital media design or network technologies. I am the lead coordinator for the [Butler Library Studio](https://studio.cul.columbia.edu/) at Columbia University Libraries, a tech-light, library innovation space focused on digital scholarship and pedagogy, and now a broadcast, [Studio Remote](https://www.twitch.tv/culstudio). I'm also co-founder and moderator of [Columbia's Group for Experimental Methods in the Humanities](http://xpmethod.plaintext.in/), a trans-disciplinary research cluster focused on experimental humanities; one of the creators and main editors of *[archipelagos journal: a journal of Caribbean digital praxis](http://archipelagosjournal.org/)*, and co-wrangler of its sister conference series, [The Caribbean Digital](http://caribbeandigitalnyc.net/). 

My research interests include Caribbean culture and history, with a focus on twentieth century poetry; digital humanities and technology design for different infrastructural and socio-economic environments; and, the relations of power and material extent of the cultural and scholarly record. 

---
<h2 id="cv"><a class="post-link" target="_blank" href="{{site.baseurl}}/docs/gil-cv.pdf">Curriculum Vitae</a>
</h2>

---

Below is a selection of my work organized by profiles---some of the different paths I walk on. Although these worlds often intersect with each other, they remain somewhat distinct to my ears, and I am often, or have been, an other Alex in each.

* TOC
{:toc}

---



## The Caribbean Digital

We did not have access to all the Caribbean literature and culture we needed to carry our studies at the University of Virginia at the beginning of the century. Maybe I could rally enough people to help build a digital library of Caribbean literature, and then... This is one of my origin stories in digital humanities: The wisdom and naivety of one day being independent and useful enough to build a digital library drove me to learn computational methods. I never did build it---thankfully others built a fine [Digital Library of the Caribbean](https://www.dloc.com/)---but I did meet enough kin spirits to help build and maintain something just as a wonderful: a support structure for a community of dialogue and practice around Caribbean digital scholarship. With Kaiama Glover and Kelly Josephs, I helped create a town hall for that community, The Caribbean Digital; with Kaiama Glover, a vehicle for it, *archipelagos*, and several wonderous examples in the genre, including "In the Same Boats." Harder to list on a profile page is the work without a project that is the community itself, shared with so many colleagues and friends. I am proud of all that we have done. Onward.

<ul class="post-list">
{% assign tcd_projects = site.data.projects | where: "category","tcd" %}
{% for project in tcd_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul> 

---

## Columbia University

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet. 

<ul class="post-list">
{% assign cu_projects = site.data.projects | where: "category","columbia" %}
{% for project in cu_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul> 

---

## Aimé Césaire

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet.

<ul class="post-list">
{% assign cesaire_projects = site.data.projects | where: "category","cesaire" %}
{% for project in cesaire_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          {% if project.link %}<a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>{% else %}<span class="post-link">{{ project.title }}</span>{% endif %}
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul>  

---

## Mobilized Humanities

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet. 

<ul class="post-list">
{% assign mobilized_projects = site.data.projects | where: "category","mobilized" %}
{% for project in mobilized_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul> 

---

## Minimal Computing

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet. 

<ul class="post-list">
{% assign minimal_projects = site.data.projects | where: "category","minimal" %}
{% for project in minimal_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul> 

---

## The Library of Babylon

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet.

<ul class="post-list">
{% assign babylon_projects = site.data.projects | where: "category","babylon" %}
{% for project in babylon_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul>  










