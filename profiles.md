---
layout: page
title: Profiles
author: Alex Gil
permalink: /profiles/
---

## Redux

I am the Digital Scholarship Librarian at Columbia University, where I collaborate with faculty, students and library colleagues in humanities research, pedagogy or knowledge production that involves the use of advanced computation, digital media design or network technologies. I am the lead coordinator for the [Butler Library Studio](https://studio.cul.columbia.edu/) at Columbia University Libraries, a tech-light, library innovation space focused on digital scholarship and pedagogy, and now a broadcast, [Studio Remote](https://www.twitch.tv/culstudio). I'm also co-founder and moderator of [Columbia's Group for Experimental Methods in the Humanities](http://xpmethod.plaintext.in/), a trans-disciplinary research cluster focused on experimental humanities; one of the creators and main editors of *[archipelagos journal: a journal of Caribbean digital praxis](http://archipelagosjournal.org/)*, and co-wrangler of its sister conference series, [The Caribbean Digital](http://caribbeandigitalnyc.net/). 

My research interests include Caribbean culture and history, with a focus on twentieth century poetry; digital humanities and technology design for different infrastructural and socio-economic environments; and, the relations of power and material extent of the cultural and scholarly record. 

Below is a copy of my curriculum vitae and a selection of some of my work. For selected open access articles, visit [the Notes section]({{site.baseurl}}/archive/). 

---
<h2><a class="post-link" target="_blank" href="{{site.baseurl}}/docs/gil-cv.pdf">Curriculum Vitae</a>
</h2>

---


## The Caribbean Digital

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet.

<ul class="post-list">
{% assign tcd_projects = site.data.projects | where: "category","tcd" %}
{% for project in tcd_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul> 

---

## For Columbia

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nec tellus mauris. Pellentesque placerat leo a laoreet consequat. Vivamus faucibus sit amet purus sagittis consectetur. Ut sagittis elit a nibh sodales, vitae scelerisque odio porttitor. Nullam dignissim tempor ante a dapibus. Aliquam erat volutpat. Aliquam laoreet, sem at aliquet tempor, augue mi sollicitudin urna, id feugiat ligula magna nec leo. Mauris egestas nulla egestas, commodo est vitae, porta elit. Aliquam mi mi, tincidunt quis bibendum vel, convallis aliquam metus. Fusce a sodales nisl. Aliquam bibendum ac leo a varius. In convallis mi non elit pharetra tempor. Morbi consectetur vulputate lectus non dignissim. Quisque egestas ullamcorper nisl, bibendum malesuada odio condimentum sit amet. 

<ul class="post-list">
{% assign cu_projects = site.data.projects | where: "category","columbia" %}
{% for project in cu_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          <a class="post-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
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
          <a class="post-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
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
          <a class="post-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
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
          <a class="post-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
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
          <a class="post-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul>  










