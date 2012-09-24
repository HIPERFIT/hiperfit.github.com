---
layout: page
title: Research Center for HIgh PERformance computing in Finance IT
---
{% include JB/setup %}

## News

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## Background

The financial sector faces computational challenges involving both an
increasing demand for performance and increasing transparency
requirements. In addition, time-to-market becomes more and more
crucial for financial applications. The joint research center HIPERFIT
attempts to solve the simultaneous challenges of high transparency,
high computational performance and high productivity in an integrated
approach of declarative domain specific and high-level functional
programming languages, gathering researchers from mathematical
finance, programming languages and high-performance systems, and
partners from the financial industry.

HIPERFIT is funded by the [Danish Council for Strategic Research
(DSF)](http://en.fi.dk/councils-commissions/the-danish-council-for-strategic-research)
under grant no. 10-092299.

