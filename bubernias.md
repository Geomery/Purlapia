---
layout: page
title: Список Буберний
permalink: /bubernias/
---

| Название Бубернии | Столица | Бубернатор | Описание флага |
| :--- | :--- | :--- | :--- |
{% for b in site.data.bubernias %}| {{ b.name }} | {{ b.capital }} | {{ b.governor }} | {{ b.flag_desc }} |
{% endfor %}
