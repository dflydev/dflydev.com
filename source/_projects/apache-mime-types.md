---
permalink: projects/apache-mime-types/
title: Apache MIME Types
tags:
    - php
github: https://github.com/dflydev/dflydev-apache-mime-types

---
{% block short_description %}

A simple interface to interacting with Apache MIME Types files.

{% endblock %}
{% block long_description %}

Parses Apache MIME Types files and provides a simple interface to find
extensions by type and type by extension.

Features
--------

 * Bundles `mime.types` from the Apache HTTP Project. ([see here][1])
 * Bundles a JSON representation of Apache `mime.types`.
 * Provides an interface for reading either flat Apache HTTP `mime.types`
   or a JSON representation.

Dragonfly Development has been invovled with this project since its inception.

{% endblock %}

[1]: https://svn.apache.org/repos/asf/httpd/httpd/trunk/docs/conf/mime.types
