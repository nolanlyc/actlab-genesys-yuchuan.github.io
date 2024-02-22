---
layout: page
permalink: /contact/
title: contact
description: 
nav: true
nav_order: 9
---

The best way to reach our team is via Slack.
Join [here](https://join.slack.com/t/genesys-cyw2842/shared_invite/zt-25q8ve5lw-h0u_bLv3fh35iivgT1qkoQ).

Additionally, the source code for GeneSys is located in the following GitHub repository.

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
