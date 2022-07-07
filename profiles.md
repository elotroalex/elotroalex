---
layout: page
title: Profiles
author: Alex Gil
permalink: /profiles/
---



<h2>In brief</h2>

Alex is Senior Lecturer II and Associate Research Faculty in Digital Humanities in the Department of Spanish and Portuguese at Yale University. He teaches introductory and advanced courses in digital humanities. His research interests include Caribbean culture and history, digital humanities and technology design for different infrastructural and socio-economic environments, and the ownership and material extent of the cultural and scholarly record. He is joint senior editor of *[archipelagos journal](http://archipelagosjournal.org/)*.   

---
<p id="cv">Download a copy of the <a class="post-link" target="_blank" href="{{site.baseurl}}/docs/gil-cv.pdf">Curriculum Vitae</a>
</p>

---

<h2>The Six Profiles</h2>

Below is a selection of my work organized by profiles---some of the different paths I walk on. Although these worlds often intersect with each other, they remain distinct enough to my ears, and I am often, or have been, an other Alex in each. Much of the work listed below is also teamwork, where I play an important role, but by no means the only important role. The dates mark my involvement in a project, not necessarily the lifespan of the project or its publication date.

* TOC
{:toc}

---



## The Caribbean Digital

We did not have access to all the Caribbean literature and culture we needed to carry our studies at the University of Virginia at the beginning of the century. Maybe I could rally enough people to help build a digital library of Caribbean literature... This is one of my origin stories in digital humanities: The wisdom and naivety of one day being independent and useful enough to build a digital library drove me to learn computational methods. I never did build it---thankfully others built a fine [Digital Library of the Caribbean](https://www.dloc.com/)---but I did meet enough kin spirits to help build and maintain something just as a wonderful: a support structure for a community of dialogue and practice around Caribbean digital scholarship. With some of my closest collaborators, I helped create a town hall for that community, The Caribbean Digital; a vehicle for it, *archipelagos*; and several wonderous examples in the genre, including "In the Same Boats" below. Harder to list on a profile page is the work without a project that is the community itself, shared with so many colleagues and friends. I am proud of all that we have done. Onward, as Kaiama says.

<ul class="post-list">
{% assign tcd_projects = site.data.projects | where: "category","tcd" %}
{% for project in tcd_projects %}
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

## The University 

Before joining Yale as faculty, I worked at Columbia University as a digital scholarship librarian for 10 years. This profile will soon evolve to reflect my contributions to Yale University. 

I was hired at Columbia University Libraries to "coordinate," to un-silo much of what was already being recognized as digital humanities activities across campus. The hire was a shard of light, bringing me into a subject specialist team, Humanities & History, rather than a digital scholarship center. If my main job was to help build community and bridges with faculty and students, I was meant to do it side-by-side with my librarian colleagues. Although I did move on to other parts of the organization, that initial setup provided the foundation for what grew later. The Studio, the xpmethods group, and many of the projects you see listed below come from the understanding that subject matter and intellectual community, not functional expertise, should be our guiding light. After almost a decade, we have been able to place our work at Columbia University on the national and international map. We have developed our own unique reconciliation between the three branches of digital humanities as I see them: architectures of knowledge, algorithmic approaches to corpora and  socio-technical mobilization. At the library, the experimental work we have fostered has quietly and beneficially filtered to other parts of the organization... and yes, we are much less siloed today.

<ul class="post-list">
{% assign cu_projects = site.data.projects | where: "category","columbia" %}
{% for project in cu_projects %}
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

## Aimé Césaire

I went to graduate school to study James Joyce and Samuel Beckett, and ended up writing a dissertation on Aimé Césaire. I really can't pinpoint the moment or specific reasons that drew me to Césaire. When I was able to identify and bring attention to Césaire's lost play about the Haitian Revolution, though, I knew my fate was sealed. In a sense, Césaire picked me, not the other way around. Delving into the broken record, asking and answering new research questions about the great poet and statesman provides the connecting tissue for what I do---where form and content crystallize for me---the fight for dignity in entanglement, but against assimilation---the restitution of poetic knowledge over a mechanistic universe. Still glad he found me.

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

In addition to the familiar avenues of teaching, advocacy, protest or democratic participation, I believe we can put to use our skills and knowledge to address the crises of our time. Sometimes in order to do so, all we need to do is reimagine how we work with each other. Perhaps we have locked ourselves into some unnecessary corners because of the institutional structures we inherit: to collaborate outside our home institutions, for example, we expect time-consuming grants; to collaborate internally, we often forgo a team better suited to the task at hand. In the meantime, crises are made more numerous and intense by that inter-connectedness that brings most things home—that inter-connectedness that shares the fuel with the <span style="  overflow-wrap: break-word; word-wrap: break-word; -ms-hyphens:auto; -moz-hyphens: auto; -webkit-hyphens: auto; hyphens: auto;">capitalopatricolonial-anthropoclusterfuckocene</span>. Perhaps it is time we learn new ways to mobilize the humanities and scholarship---in their glorious differences from natural science---to face our collective urgencies. We may not be able to have the same "impact" as industry, and its academic arm, without matching the funding levels they command, but that does not mean we're devoid of consequential power. Below are some team efforts that I have been a part of, meant to develop the muscle memory to assemble in new keys, new registers, bringing often little or no coin, but always each other and what we already know.

<ul class="post-list">
{% assign mobilized_projects = site.data.projects | where: "category","mobilized" %}
{% for project in mobilized_projects %}
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

## Minimal Computing


The digital divide works less like a two-sided coin, and more like intersecting ecologies. This is what we can observe around the world, from New York City's Rikers Island jail, where the guards have exclusive access to machines, but our young remember them; to the sneakernets in Havana for LGBTQ or critical race scholarship, or the strange Tlön, Uqbar, Orbis Tertius of their intranet; to the afternoons at the University of Khartoum, when the internet is faster and the lights are on, but the government is still... you know. How then do we build and maintain our scholarly edifices for a world with these differences? This is the main driver behind "minimal computing": to lower the overall costs of scholarly digital production, sharing and stewardship across as many registers as we can perceive and describe... to meet our most basic needs as scholars and teachers: to understand and tweak the past for those who come after us. 


<ul class="post-list">
{% assign minimal_projects = site.data.projects | where: "category","minimal" %}
{% for project in minimal_projects %}
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

## The Broken Record

What is the actual shape of the world's archive? I have a recurring daydream of all existing documents in the world---analog and digital---from the codices dormant in warehouses, to the algorithms and data waiting for a reader to summon their outputs into being. Even if the amount is hard to count at any given moment, like swallows flying by, it may still be finite. <!-- This is the opposite of Borges' Library of Babel, which has randomly generated sequences of characters, most volumes are nonsense, is definitely closer to infinity, and can only ever be but a computational document to us. --> How are we to understand it's shape? With what macroscopes? The computational? The postcolonial? Maybe breaking it down into corners might make the task easier. We know, for example, that a few for-profit monopolies have come to control that corner we call the scholarly record of the North Atlantic world; that pirate libraries do their caring by freeing that knowledge production, in many cases for the benefit of a grateful Global South, whose own mom-and-pop, or government-subsidized production, still remains mostly invisible to that North Atlantic. And what of the myriad other ways in which our record is found already broken because of our post-1492 world: the produced silences of the colonial past, or the accidental ones? The stolen volumes? Or the piles of useless ones? I see the desire to make that record whole by owning it, and with these desires much grief.  I daydream instead of mending the wounds of the past and present---and fighting for the future---of our de facto Library of Babylon---a library ultimately made for immigrants and exiles, in imperfectly translatable tongues, steadily refracted by annotation, rife with gaps for us to hide in, and impossible to control by sameness.

<ul class="post-list">
{% assign babylon_projects = site.data.projects | where: "category","babylon" %}
{% for project in babylon_projects %}
    <li>
        <span class="post-meta">{{ project.time }}</span>
        <h3>
          {% if project.link %}<a class="post-link" target="_blank" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>{% else %}<span class="post-link">{{ project.title }}</span>{% endif %}
        </h3>
        <span>{{ project.blurb }}</span>
    </li>
{% endfor %}
</ul>  










