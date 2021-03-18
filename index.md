---
layout: default
title: Ricardo Silva
---

---

## About me
📍 {{ site.data.bio.location }}

ℹ️ {{ site.data.bio.about }}

## Goals

{% for goal in site.data.goals %}
- [{{ goal.name }}]({{ goal.link }})
{% endfor %}

## Jobs

{% for job in site.data.jobs %}
### {{ job.name }}
📅 {{ job.when }}
{% for what in job.what %}
- 🛠 {{ what }}
{% endfor %}
🏢 [{{ job.where.name }}]({{ job.where.link }}])

💡 {{ job.lesson }}
{% endfor %}

## Skills

{% for skillset in site.data.skillsets %}
### {{ skillset.name }}
{% for keyword in skillset.keywords %}
- {{ keyword }}
{% endfor %}
{% endfor %}
