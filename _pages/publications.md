---
layout: page
permalink: /publications/
title: publications
description: My publications can also be found on my [Google Scholar](https://scholar.google.com/citations?user=kVyW-LEAAAAJ) and [Research Gate](https://www.researchgate.net/profile/Efi-Psomopoulou) profiles.
years: [2021, 2020, 2019, 2018, 2017, 2015, 2014, 2012]
nav: true
---

<div class="publications">

 {% for y in page.years %}
   <h2 class="year">{{y}}</h2>
   {% bibliography -f papers -q @*[year={{y}}]* %}
 {% endfor %}
 
</div>
