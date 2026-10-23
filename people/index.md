---
title: People
nav:
  order: 2
  tooltip: Lab members and alumni
redirect_from:
  - /team/
---

# Lab Members

{% assign members = site.members | sort: "name" %}
{% assign pi = members | where: "role", "principal-investigator" | first %}

{% include team-member.html member=pi pi=true %}

{% include section.html %}

{% assign phd = members | where: "role", "phd" %}
{% assign ms = members | where: "role", "ms" %}
{% assign undergrad = members | where: "role", "undergrad" %}

{% if phd.size > 0 %}
## PhD Students

{% for m in phd %}{% include team-member.html member=m %}{% endfor %}
{% endif %}

{% if ms.size > 0 %}
## Master's Students

{% for m in ms %}{% include team-member.html member=m %}{% endfor %}
{% endif %}

{% if undergrad.size > 0 %}
## Undergraduate Students

{% for m in undergrad %}{% include team-member.html member=m %}{% endfor %}
{% endif %}

{% assign affiliates = members | where: "role", "affiliated" %}
{% if affiliates.size > 0 %}
## Lab Affiliates

{% for m in affiliates %}{% include team-member.html member=m %}{% endfor %}
{% endif %}

{% include section.html %}

## Past Lab Members {#alumni}

Alumni have joined Google, Amazon, the NIH, Panasonic, Oracle, Allstate, GoHealth and Procured Health, and gone on to graduate study at Northwestern, Northeastern, Carnegie Mellon and the University of Illinois Chicago.

{% include alumni-logos.html %}

{% include alumni.html %}
