---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======

<!-- EXERCISE: Reproduce this education section with Liquid code using "includes" and custom data files!
If time permits, also add a bullet for supervisors -->

{% assign education_data = site.data.education | sort: "year_start" %}

<!-- In Markdown: -->
<!-- {% for item in education_data %}
  {% include education-item-cv.md %}
{% endfor %} -->

<!-- In HTML: -->
<ul>{% for item in education_data %}
  {% include education-item-cv.html %}
{% endfor %}</ul>

<!-- EXERCISE: If time permits, fill in the rest of this CV with your own data -->

Work experience
======
* Summer 2015: Research Assistant
  * Github University
  * Duties included: Tagging issues
  * Supervisor: Professor Git

* Fall 2015: Research Assistant
  * Github University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub

Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Service and leadership
======
* Currently signed in to 43 different slack teams
