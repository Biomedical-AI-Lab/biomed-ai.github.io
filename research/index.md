---
title: Research
nav:
  order: 1
  tooltip: Research areas, grants, software and data
redirect_from:
  - /software/
  - /projects/
  - /apps/
  - /funding/
  - /grants/
---

# Research in the Biomedical AI Lab

{% assign domains = site.data.highlights %}

We build machine learning that clinicians can use: models that score movement, detect falls, read clinical text and interpret medical images. Below are highlights from each area, the grants that fund our work, and the software and data we share.
{:.page-sub}

<div class="jump-links">
{%- for d in domains -%}<a href="#{{ d.id }}">{{ d.label }}</a>{%- endfor -%}
<a class="jump-strong" href="#grants">Grants</a><a class="jump-strong" href="#software">Software &amp; Data</a>
</div>

{% for d in domains %}
{% include section.html %}

<h2 class="area-title" id="{{ d.id }}"><i class="{{ d.icon }}" aria-hidden="true"></i>{{ d.title }}</h2>

<p class="focus-line">{{ d.focus }}</p>

<div class="rcard-grid">
{%- for it in d.items -%}
<article class="rcard" data-theme="{{ d.id }}"><div class="rcard-top"><span class="rcard-icon"><i class="{{ d.icon }}" aria-hidden="true"></i></span><span class="rcard-venue">{{ it.venue }}</span></div><h3 class="rcard-title">{{ it.title }}</h3><p class="rcard-text">{{ it.text }}</p><div class="tag-row">{%- for tg in it.tags -%}<span class="tag-pill">{{ tg }}</span>{%- endfor -%}</div>{%- if it.link -%}<div class="text-links"><a href="{{ it.link }}">Read the paper <i class="fa-solid fa-arrow-right" aria-hidden="true"></i></a></div>{%- endif -%}</article>
{%- endfor -%}
</div>
{% endfor %}

{% include section.html %}

<h2 id="grants"><i class="fa-solid fa-sack-dollar" aria-hidden="true"></i>Grants and funding</h2>

Our research is supported by federal agencies, children's hospitals, foundations and the university. Every award Dr. Albert has led or joined is listed below with its amount.

{% include grants.html %}

<p class="partner-label">Grant providers</p>
{% include partner-logos.html type="sponsor" %}

<p class="partner-label">Collaborators</p>
{% include partner-logos.html type="collaborator" %}

{% include section.html %}

<h2 id="software"><i class="fa-solid fa-laptop-code" aria-hidden="true"></i>Software and data</h2>

Apps, notebooks and tools from the lab. Each card links to the app, the paper or the code.

<div class="scard-grid">
{%- for p in site.data.projects -%}
<article class="scard"><h3 class="scard-title"><a href="{{ p.link }}">{{ p.title }}</a></h3><span class="scard-sub">{{ p.subtitle }}</span><div class="scard-text">{{ p.description | markdownify }}</div><div class="tag-row">{%- for tg in p.tags -%}<span class="tag-pill">{{ tg }}</span>{%- endfor -%}</div></article>
{%- endfor -%}
</div>

**In the works:** a dashboard for music-induced hearing loss, topic modeling, a biomarker detection app, stock2vec and a dual reinforcement learning app. Each gets a card here once its link or code is public.

{% include section.html %}

## All of our work

These are highlights only. For the complete, up-to-date list of papers and citations, see Prof. Albert's Google Scholar profile.

<div class="cta-row">
<a class="cta" href="https://scholar.google.com/citations?user=LPzMx1IAAAAJ&view_op=list_works&sortby=pubdate">Google Scholar</a>
<a class="cta ghost" href="{{ "publications" | relative_url }}">Selected publications</a>
</div>
