---
permalink: projects/git-subsplit/
title: git-subsplit
tags:
    - bash
github: https://github.com/dflydev/git-subsplit

---
{% block short_description %}

Automate and simplify the process of managing one-way read-only subtree splits.

{% endblock %}
{% block long_description %}

One-way read-only subtree splits can be used to split components from a combined repository into their own standalone repository.
This was made popular by several large PHP frameworks, notably Symfony.

This project is currently written in bash and relies on `git subtree`.

This works well for smaller projects but after a certain point the process may become slower than desired.

Dragonfly Development has been invovled with this project since its inception.

{% endblock %}
