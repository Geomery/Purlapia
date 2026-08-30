---
layout: page
title: Постановления Совета Буберний
permalink: /decrees/
---

{% for decree in site.data.decrees %}
### Постановление №{{ decree.number }} (от {{ decree.date }})
* **Тема:** {{ decree.title }}
* **Голоса:** {{ decree.status }}
* **Текст:** {{ decree.text }}

---
{% endfor %}
