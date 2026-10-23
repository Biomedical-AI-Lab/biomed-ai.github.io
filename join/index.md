---
title: Join Us
nav:
  order: 6
  tooltip: Prospective students
redirect_from:
  - /prospective-students/
---

# Join Us

{% assign brand = site.data.affiliation %}
{% if site.recruiting %}
<div class="recruiting-banner">We are actively recruiting students to lead or contribute to ongoing projects.</div>
{% else %}
<div class="status-note"><strong>We are not actively recruiting new students at the moment.</strong><br>Exceptional PhD applicants may still reach out as described below. This page will announce new openings.</div>
{% endif %}

{% include section.html %}

## PhD students

### What we look for

- **Foundations:** a BS or MS in computer science, computer engineering, electrical or biomedical engineering, statistics or a related field, with solid linear algebra, probability, statistics and optimization.
- **Modern machine learning:** hands-on deep learning in PyTorch or JAX, including training and fine-tuning transformers, large language models or vision-language models; comfort with Linux, git, GPU clusters and reproducible experiments.
- **Evidence of research:** a first-author paper or preprint, a strong thesis, or substantial open-source code. Work at venues such as NeurIPS, ICML, ICLR, ACL, EMNLP, CVPR, MICCAI, KDD, IEEE JBHI or IEEE ICHI stands out.
- **Health and real-world data:** genuine interest in clinical data such as wearable signals, gait, clinical text and medical images, and in responsible, privacy-aware AI.
- **Communication:** clear scientific writing and presenting, and meeting the graduate school's English requirements.
- **Commitment:** full-time research aimed at top venues, typically over four to five years.

### How to apply

1. Apply to the Computer Science and Engineering or Information Science PhD program at {{ brand.short_name }}.
2. After you apply, email Prof. Albert at [{{ site.links.email }}](mailto:{{ site.links.email }}) with your **application number**, your CV, the research area above you want to work in, and links to your papers and code.
3. Promising candidates may be invited for an interview.

Funding is limited. Teaching assistantships come through the department, and research assistantships depend on current grants.

{% include section.html %}

## MS, Undergraduate and TAMS students

You do not need research experience to join. The requirements below are what usually works best, but **we are flexible**: if you miss one of them, reach out anyway and tell us what you can offer.

### What we ask

- **Time:** about 10 to 15 hours a week. We can work around exams and heavier semesters.
- **Commitment:** at least 1.5 years with the lab, so that you have time to learn the project and finish something you are proud of. For that reason we usually do not take students in their final year; if you are close to graduating, mention it and we can talk.
- **Programming:** you should program confidently in Python.
- **Coursework:** at least one machine learning or data science course. A well-documented online course or self-study project can also count.

### What is not required

- **Publications or prior research.** We will teach you how to read papers, run experiments and present results.
- **A computing major.** Students from biology, kinesiology, health sciences, engineering and other fields are welcome, especially if you care about health data.
- **A fixed project idea.** Most new students start by helping on an ongoing project.

### By program

- **MS students** usually start by assisting on a project and can propose their own with ML experience and more than a year left in their program. RA funding is usually not available.
- **Undergraduates** most often join through the AI Summer Research Program or after an open house.
- **TAMS students** are welcome under the same expectations. If you have not taken a machine learning course yet, a Python project or online course is enough to start.

### How to join

1. **Come to an open house.** They run 3:00 to 5:00 pm on the Thursday the week before each fall and spring semester, at {{ brand.address.building }}. New students generally join in the first week of classes, after an open house.
2. **Or join the AI Summer Research Program**, the main route for undergraduate and MS students. It starts in late May and presents progress in late June. Contact Prof. Albert for details.
3. **Or email Prof. Albert** at [{{ site.links.email }}](mailto:{{ site.links.email }}) with your program and year, a short CV, the hours you can give each week, and a sentence or two on what interests you.

{% include section.html %}

## Summer research

- **AI Summer Research Program.** Created and co-directed by Prof. Albert; since 2020 it has engaged 239 students in 75 projects, with about 9 faculty advisors each summer.
- **NSF REU Site: Making Generative AI Responsible** (2025–2028): paid summer research for undergraduates.
- **Advancing Digital Health Technology** (NIH, 2025–2030): a summer research program for high school and community college educators.

See the [alumni list]({{ "people" | relative_url }}#alumni) for where our former students went next.
