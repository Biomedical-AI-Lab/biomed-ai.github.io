---
title: Contact
nav:
  order: 7
  tooltip: Email, address and location
---

# Contact

{% assign brand = site.data.affiliation %}

{% include section.html %}

<div class="focus-grid">
<div markdown="1">

#### <i class="fa-solid fa-flask"></i>Lab

**{{ site.title }}**  
Room {{ brand.address.lab_room }}, {{ brand.address.building }}  
{{ brand.address.street }}  
{{ brand.address.city }}

[Directions on Google Maps]({{ brand.address.map }})

</div>
<div markdown="1">

#### <i class="fa-solid fa-user-tie"></i>Principal Investigator

**Dr. Mark V. Albert**  
Office {{ brand.address.pi_office }}, {{ brand.address.building }}  
[{{ site.links.email }}](mailto:{{ site.links.email }}) (email preferred)

</div>
</div>

Prospective students: please see [Join Us]({{ "join" | relative_url }}) and come to an open house rather than visiting unannounced.
