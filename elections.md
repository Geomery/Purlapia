---
layout: page
title: Выборы Народного Депутата
permalink: /elections/
---
## **Действующий народный депутат: {{ election.now }}**
{% for election in site.data.elections %}
### Выборы №{{ election.number }}
* **Дата:** {{ election.date }}
* **Народный Депутат:** **{{ election.winner }}**

**Результаты голосования:**
{% for candidate in election.candidates %}
* {{ candidate.name }} — {{ candidate.votes }} голосов
{% endfor %}

---
{% endfor %}
