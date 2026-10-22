---
title: People
nav:
  order: 3
  tooltip: Lab members and alumni
redirect_from:
  - /team/
---

# {% include icon.html icon="fa-solid fa-users" %}People

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}

{% include section.html %}

## PhD students

{% include list.html data="members" component="portrait" filter="role == 'phd'" %}

## MS students

{% include list.html data="members" component="portrait" filter="role == 'ms'" %}

## Undergraduate students

{% include list.html data="members" component="portrait" filter="role == 'undergrad'" %}

## Lab affiliates

{% include list.html data="members" component="portrait" filter="role == 'affiliated'" %}

{% include section.html %}

## Alumni

Where our former students went next.

{% include alumni.html %}
