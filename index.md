---
---

{% assign brand = site.data.affiliation %}

{% if site.construction-notice %}<div class="recruiting-banner construction-notice">Website Under Construction</div>{% endif %}

<div class="hero">
<img src="{{ "images/logo.png" | relative_url }}" alt="{{ site.title }} logo">
<div>
<h1>{{ site.title }}</h1>
<p>{{ brand.department }} · {{ brand.institution }}</p>
</div>
</div>

We use **machine learning to advance medicine**. Our roots are in **wearable-device analytics** that help clinicians treat mobility disorders, and today we build **movement, sensing, language and imaging models** that measure health outcomes more precisely, to address mobility impairment including **Parkinson's disease, cerebral palsy, stroke, amputation and spinal cord injury**.

<div class="focus-grid" markdown="1">
<div markdown="1">

#### <i class="fa-solid fa-person-walking"></i>Movement and Gait

- **Gait quality scores:** the Shriners Gait Index for children with cerebral palsy.
- **Clinical prediction:** surgical outcomes and fall risk from gait and balance data.
- **Rehabilitation outcomes:** precise measurement of prosthetic performance, spasticity, Parkinson's symptoms and more.

</div>
<div markdown="1">

#### <i class="fa-solid fa-mobile-screen"></i>Wearable Sensing

- **Fall risk prediction:** phones and wearables that flag risk early, and airbag belts that respond in real time.
- **Activity recognition and assessment:** from toddlers to adults with spinal cord injury.
- **Gesture-to-speech:** wearable gesture recognition for people who cannot speak.

</div>
<div markdown="1">

#### <i class="fa-solid fa-comment-medical"></i>Language Models

- **Clinical text:** fall risk and pain assessment from medical records.
- **Humanitarian NLP:** human-rights annotation and conflict forecasting.
- **Trustworthy LLMs:** explainability, distillation and cross-lingual bias.

</div>
<div markdown="1">

#### <i class="fa-solid fa-x-ray"></i>Multimodal and Imaging AI

- **Radiology:** multi-agent report generation and visual question answering.
- **Vision-language models:** small, efficient models for clinical settings.
- **Foundations:** brain-inspired, efficient-coding models of perception.

</div>
</div>

<div class="cta-row">
<a class="cta" href="{{ "research" | relative_url }}">Research highlights</a>
<a class="cta ghost" href="{{ "publications" | relative_url }}">Publications</a>
</div>

{% include section.html %}

#### Our impact

Our work appears in venues including **IEEE JBHI, Journal of Biomechanics, Journal of NeuroEngineering and Rehabilitation, PLoS Computational Biology, Information Fusion, JMIR Medical Informatics, ECML PKDD, IJCAI, LREC, ACM/IEEE JCDL and IEEE ICHI**, and in two US patents.

#### Grant providers and collaborators

Our work is funded by federal agencies, children's hospitals and foundations. [See all grants and amounts →]({{ "research" | relative_url }}#grants)

<p class="partner-label">Grant providers</p>
{% include partner-logos.html type="sponsor" %}

<p class="partner-label">Collaborators</p>
{% include partner-logos.html type="collaborator" %}

#### Join us

{% if site.recruiting %}<div class="recruiting-banner">We are actively recruiting students to lead or contribute to ongoing projects.</div>{% else %}We are not actively recruiting at the moment. Exceptional PhD applicants can still reach out. See **[Join Us]({{ "join" | relative_url }})** for how to apply and what we look for.{% endif %}

{% include section.html %}

#### Latest news

{% include news-list.html limit=5 %}

[All news →]({{ "news" | relative_url }})
