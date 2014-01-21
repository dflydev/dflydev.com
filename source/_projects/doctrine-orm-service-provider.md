---
permalink: projects/doctrine-orm-service-provider/
title: Doctrine ORM Service Provider
tags:
    - php
    - doctrine
    - silex
    - pimple
    - cilex
github: https://github.com/dflydev/dflydev-doctrine-orm-service-provider

---
{% block short_description %}

Provides Doctrine ORM Entity Managers as services to Pimple applications.

{% endblock %}
{% block long_description %}

Provides Doctrine ORM Entity Managers as services to
[Pimple](http://pimple.sensiolabs.org/) applications. Adapters are provided for
both [Silex](http://silex.sensiolabs.org/) and [Cilex](http://cilex.github.io/).

If you are not familiar with Doctrine ORM, it is a high quality Object
Relational Mapper (ORM) for PHP. It sits on top of a powerful database
abstraction layer (DBAL). While the jury is still out on whether [using an ORM
is a good thing or a bad thing](http://www.codinghorror.com/blog/2006/06/object-relational-mapping-is-the-vietnam-of-computer-science.html),
it is extremely popular in some circles.

It should be no secret that we are a fan of [Silex](http://silex.sensiolabs.org/), so when we wanted to leverage Doctrine ORM in our Silex projects we came up empty.

So we wrote a Silex service provider ourselves.

Based on the core [Doctrine Service Provider](http://silex.sensiolabs.org/doc/providers/doctrine.html),
Doctrine ORM Service provider exposes Entity Managers in a way that is easy to
configure and use. Symfony 2 users will appreciate the ability to use Doctrine
ORM entities in Silex as easily as they can in their Symfony 2 applications.

<br>

Would your business benefit from integrating Doctrine ORM into your Pimple, Silex, or Cilex applications? [Contact us]({{site.url}}/contact/) to see how we can help.

{% endblock %}
