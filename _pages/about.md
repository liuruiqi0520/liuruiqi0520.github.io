---
permalink: /
title: "Jerry H. Liu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I am Jerry. I am a second-year Ph.D. student in Computer Science at the University of Illinois Urbana-Champaign (UIUC), advised by [Prof. Nan Jiang](https://njiang.cs.illinois.edu/).

My research interest lies in reinforcement learning, specifically in offline reinforcement learning, representation learning and foundation models.

You can reach me at `jerryhdliu [at] illinois [dot] edu`.

For more information, please see my [CV]({{ site.baseurl }}/files/CV_JerryLiu.pdf), [Google Scholar](https://scholar.google.com/citations?user=1cIAMNMAAAAJ), [GitHub](https://github.com/jerryhdliu), and [LinkedIn](https://www.linkedin.com/in/jerryhdliu/).

## News
{% assign posts_collate = site.posts | where_exp: "item", "item.hidden != true" | sort: "date" | reverse %}
{% for post in posts_collate limit:5 %}
  {% include archive-single.html type="list" %}
{% endfor %}
<p style="margin-top: 1em; text-align: right;"><a href="{{ site.baseurl }}/posts/">Read more posts &raquo;</a></p>

## Selected Publications
{% assign selected_publications = site.publications | where: "selected", "true" | sort: "date" | reverse %}
{% for pub in selected_publications %}
  {% include archive-single-cv.html %}
{% endfor %}
<p style="margin-top: 1em; text-align: right;"><a href="{{ site.baseurl }}/publications/">All publications &raquo;</a></p>

## Teaching
{% assign teaching_sorted = site.teaching | sort: "year" | reverse %}
{% for course in teaching_sorted %}
  {% include archive-single.html %}
{% endfor %}
<p style="margin-top: 1em; text-align: right;"><a href="{{ site.baseurl }}/teaching/">All teaching &raquo;</a></p>

