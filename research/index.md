---
title: Research
nav:
  order: 1
  tooltip: Research highlights
---

# Research in the Biomedical AI Lab

{% assign domains = site.data.highlights %}

We build machine learning that clinicians can use: models that score movement, detect falls, read clinical text and interpret medical images. Below are a few highlights from each area.
{:.page-sub}

<div class="jump-links">
{%- for d in domains -%}<a href="#{{ d.id }}">{{ d.label }}</a>{%- endfor -%}
</div>

{% for d in domains %}
{% include section.html %}

<span class="kicker" id="{{ d.id }}"><i class="{{ d.icon }}" aria-hidden="true"></i>&nbsp; {{ d.label }}</span>

### {{ d.title }}

<p class="focus-line"><strong>Focus:</strong> {{ d.focus }}</p>

<div class="highlight-grid">
{%- for it in d.items -%}
<article class="highlight">{% include theme-thumb.html theme=d.id image=it.image %}<div class="highlight-body"><h4>{{ it.title }}</h4><span class="venue">{{ it.venue }}</span><p>{{ it.text }}</p><div class="tag-row">{%- for tg in it.tags -%}<span class="tag-pill">{{ tg }}</span>{%- endfor -%}</div>{%- if it.link -%}<div class="text-links"><a href="{{ it.link }}">[Paper]</a></div>{%- endif -%}</div></article>
{%- endfor -%}
</div>
{% endfor %}

{% include section.html %}

## All of our work

These are highlights only. For the complete, up-to-date list of papers and citations, see Prof. Albert's Google Scholar profile.

<div class="cta-row">
<a class="cta" href="https://scholar.google.com/citations?user=LPzMx1IAAAAJ&view_op=list_works&sortby=pubdate">Google Scholar</a>
<a class="cta ghost" href="{{ "publications" | relative_url }}">Selected publications</a>
</div>

<details class="alumni-group" markdown="1">
<summary>Funding: current and recent projects</summary>

| Project | Sponsor | Role | Years |
| --- | --- | --- | --- |
| Predicting and Optimizing Long-Term Outcomes in Pediatric-Onset Spinal Cord Injury | Shriners Children's | Site PI | 2026–2027 |
| Advancing Digital Health Technology: A Summer Research Program for Educators | NIH (R25) | Co-PI | 2025–2030 |
| REU Site: Making Generative Artificial Intelligence Responsible | NSF | Co-PI | 2025–2028 |
| Precision gesture-to-speech system for speech-impaired individuals with limited mobility | C-STAR, Shirley Ryan AbilityLab (NIH) | Subcontract | 2024 |
| Improving Orthopaedic Outcomes through Machine Learning | Shriners Children's | Site PI | 2023–2026 |
| Using the Fitbit for Early Detection of Infection after Discharge in Pediatric Surgical Patients | NIH (R01), with Lurie Children's Hospital | Co-I | 2023–2027 |
| Predicting Fall Risk in Older Adults Using Machine Learning | Johns Hopkins AITC for Aging Research, with UNT Health Science Center | Subaward | 2023–2024 |
| Hierarchically Structured Materials Systems for Enhanced Dynamic Performance | U.S. Army Research Laboratory | Co-PI | 2023–2024 |
| AI4All College Pathways | AI4All | Co-PI | 2022–2023 |
| Physical Activity Measurement in Toddlers | NIH (R01), with Lurie Children's Hospital | Co-I | 2021–2026 |
| REU Site: Accelerated Deep Learning through a Hardware-Software Collaborative Approach | NSF | Co-PI | 2021–2023 |
| Fall Catcher: Wearable Airbag Technology to Mitigate Falls after Stroke | RERC, with Shirley Ryan AbilityLab | Subcontract | 2018–2023 |

</details>

**Collaborators:** Shriners Children's · Shirley Ryan AbilityLab · Lurie Children's Hospital of Chicago · UNT Health Science Center · Northwestern University
