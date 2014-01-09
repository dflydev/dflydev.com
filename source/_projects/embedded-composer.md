---
permalink: projects/embedded-composer/
title: Embedded Composer
tags:
    - php
    - composer
github: https://github.com/dflydev/dflydev-embedded-composer

---
{% block short_description %}

Embed [Composer](http://getcomposer.org/) into another application.

{% endblock %}
{% block long_description %}

Imagine a console application shipped as a phar. If it is desired for the
application to be extensible based on which directory it is in (say one set
of plugins should be used in one directory but an entirely different set of
plugins used in another directory) one cannot simply define a `composer.json`
in both directories and run `composer install`.

Why not? Because the application shipped with a specific set of dependencies.
Composer cannot add more dependencies without running the risk of introducing
conflicts. The answer is to embed Composer into the application so that
Composer can merge the dependencies already installed for the application
with the dependencies defined in a specific directory's `composer.json`.

The end result is a set of dependencies that satisfy the directory specific
requirements while taking into account the dependencies *already installed*
for the console application.

While this is required for a phar distributed application this technique can
be applied to any globally installed application that needs to be runtime
extensible.

This project is aimed at enabling developers to embed
[Composer](http://getcomposer.org/) into another application and alleviate the
problems laid out here.

Used extensively by [Sculpin]({{site.url}}/projects/sculpin/).

Dragonfly Development is responsible for creating and maintaining this project.

{% endblock %}
