---
---

# Biomedical AI Lab

We use machine learning to advance medicine.
Our roots are in wearable-device analytics that help clinicians treat mobility disorders, and our work now spans movement, sensing, language and imaging models for health.

{%
  include button.html
  link="research"
  text="Our research"
  icon="fa-solid fa-arrow-right"
  flip=true
%}
{%
  include button.html
  link="join"
  text="Join the lab"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% include section.html %}

## Research themes

{% include themes.html %}

{% include section.html %}

## Populations we study

<div class="chip-row">
<span class="chip">Parkinson's disease</span>
<span class="chip">Incomplete spinal cord injury</span>
<span class="chip">Transfemoral amputation</span>
<span class="chip">Cerebral palsy</span>
<span class="chip">Stroke</span>
<span class="chip">Toddlers</span>
</div>

{% include section.html %}

## Featured papers

{% include list.html data="citations" component="citation" style="rich" filter="tags && tags.include?('featured')" %}

{%
  include button.html
  link="publications"
  text="All publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}
{:.center}

{% include section.html %}

## Latest news

{% for post in site.posts limit: 5 %}
- **{{ post.date | date: "%b %-d, %Y" }}**: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

{%
  include button.html
  link="news"
  text="All news"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}
{:.center}

{% include section.html dark=true %}

## Join us

We welcome undergraduate, MS and PhD students with strong programming skills and an interest in AI for health.
Open houses run the Thursday before each fall and spring semester at {{ site.data.affiliation.address.building }}.

{%
  include button.html
  link="join"
  text="How to join"
  icon="fa-solid fa-arrow-right"
  flip=true
%}
{:.center}
