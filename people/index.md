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

## PhD Students

{% for m in members %}{% if m.role == "phd" %}{% include team-member.html member=m %}{% endif %}{% endfor %}

## Master's Students

{% for m in members %}{% if m.role == "ms" %}{% include team-member.html member=m %}{% endif %}{% endfor %}

## Undergraduate and TAMS Students

{% for m in members %}{% if m.role == "undergrad" %}{% include team-member.html member=m %}{% endif %}{% endfor %}

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
