---
layout: default
title: Ricardo Silva
---

---

![profile picture](assets/images/profile_picture_border.jpeg)

[![profile picture](assets/images/logo_github_mark.png)](https://github.com/ohCancio)
[![profile picture](assets/images/logo_linkedin_ln.png)](https://www.linkedin.com/in/ricardo-c%C3%A2ncio-silva-43860830/)
[![profile picture](assets/images/logo_twitter_social.png)](https://twitter.com/ohCancio)

## About me
📍 {{ site.data.bio.location }}

{{ site.data.bio.about }}

## Goals

{% for goal in site.data.goals %}
- [{{ goal.name }}]({{ goal.link }})
{% endfor %}

## Jobs

{% for job in site.data.jobs %}
### {{ job.name }}
📅 {{ job.when }} {% if job.where.link %}
🏢 [{{ job.where.name }}]({{ job.where.link }})
{% else %}
🏢 {{ job.where.name }}
{% endif %}

{% for what in job.what %}
- {{ what }}
{% endfor %}

💡 {{ job.lesson }}
{% endfor %}

## Skills

{% for skillset in site.data.skillsets %}
### {{ skillset.name }}
{% for keyword in skillset.keywords %}
- {{ keyword }}
{% endfor %}
{% endfor %}

---
