---
layout: page
title: Выборы Народного Депутата
permalink: /elections/
---

## **Действующий Народный Депутат: Кто-то**
{% for election in site.data.elections %}
### Выборы №{{ election.number }}
* **Дата:** {{ election.date }}
* **Народный Депутат:** **{{ election.winner }}**

**Результаты 1 тура:**
{% for candidate in election.candidates %}
* {{ candidate.name }} — {{ candidate.votes }} голосов
{% endfor %}

{% if election.round2 %}
**Результаты 2 тура:**
{% for candidate in election.round2.candidates %}
* {{ candidate.name }} — {{ candidate.votes }} голосов
{% endfor %}
{% endif %}

---
{% endfor %}
