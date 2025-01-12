---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
This page includes a timeline of my Education and career, and a highliht of my skills accumulated over the years. <br>
I am currently a senior at UC Berkeley graduating in fall 2025. I am passionate about mechanics and space technology. 

<div class="row">
{% include about/skills.html title="Software Skills" source=site.data.software-skills %}
{% include about/skills.html title="Technical Skills" source=site.data.technical-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>