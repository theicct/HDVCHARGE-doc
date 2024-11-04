---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: HDV CHARGE Model Documentation
---

The electrification of medium-duty and heavy-duty vehicles (MHDVs) is crucial for achieving climate goals and mitigating the health impacts of air pollution. Electric charging and hydrogen refueling infrastructure are key not only for advancing market developments but also for enabling vehicle-side policies. A precise understanding of energy and power requirements—how much, where, and when—is essential, alongside a clear grasp of the number of chargers needed to supply it. This information is vital for informing stakeholders about the deployment of chargers and necessary upgrades to electric transmission and distribution grids.

To inform this complex task, the ICCT developed the HDV CHARGE model. HDV CHARGE is a Python-based tool designed to assess charging infrastructure needs for heavy-duty vehicles (including medium-duty trucks, heavy-duty trucks, and buses) at any scale, from local (e.g., zip-code level) to supra-national (e.g., the European Union), for any market, and at any time horizon, based on specific inputs.

HDV CHARGE was first developed in 2024 by Jakob Schmidt, Nicole Egerstrom, Gabe Hillman Alvarez, and Pierre-Louis Ragon. The initial development was generously funded by the CRUX Alliance and the Aspen Global Change Institute.

## Versions

HDV CHARGE is under continuing development. Documentation of all versions since v1.0 can be found here.

{% assign pages = site.pages | sort: "title" | reverse %}
{% for page in pages %}
{% if page.dir contains '/versions/' and page.title contains 'HDV CHARGE v'%}
<li><a class="page-link" href="{{ page.url | relative_url }}">{{ page.title | escape }}</a></li>
{% endif %}
{% endfor %}
