---
layout: base
---

# Welcome!


{% for page in site.pages %}
    {% if page.event %}
{{ page.event.date }}: [**{{ page.talk.title }}**]({{ page.url }})
- Duration: {{ page.talk.duration }}
- Event: {% if page.event.link %} [{{ page.event.name }}]({{ page.event.link }}){% else %}{{ page.event.name}}{% endif %} 
- Location: {{ page.event.location }}
    {% endif %}
{% endfor %}


