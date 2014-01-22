---
permalink: projects/stackphp/
title: Stack
is_featured: true
tags:
    - php
logos:
    small: assets/projects/stack-logo.png
    large: assets/projects/stack-logo.png
website: http://stackphp.com
github: https://github.com/stackphp
twitter: stackphp

---
{% block short_description %}

Symfony HTTP Kernel middlewares.

{% endblock %}
{% block long_description %}

> Stack is a set of conventions for composing Symfony HTTP Kernel Interface applications. In addition to the conventions, Stack also provides a handful of tools that can be used to make life with Stack even easier.

We are serious about our framework agnosticism. It is our passion for this that led our team to helping start the Stack project.

What is Stack? [Whole talks have been given on the subject][3] and why it is important. Some of which can be [incredibly deep and geeky but extremely fun][4].

From the practical business side of things, Stack is a way to write and use code that operates at the HTTP level. Because it operates at the level of HTTP messages, Stack middlewares (shared pieces of code) can be used with any frameworks or applications built using Symfony's HTTP Kernel.

While this is definitely not a silver bullet for all your application needs, it *can* be extremely useful in some cases. One of the easiest examples would be trying to integrate an authentication scheme like [Hawk][1] into the API your business relies on. Before Stack, your only options would be to build Hawk authentication into your application directly or build it into an extension for your framework of choice (if one wasn't already built).

With Stack, the Hawk specific code only needs to be written once *and it works with any application for framework based on Symfony's HTTP Kernel*. This means that you can add Hawk functionality to any Symfony, Silex, Laravel, or Drupal 8 project simply by adding the [Stack Hawk][1] middleware to your stack. Your API is now secured by Hawk, and you did it without having to change much at all about your application or the framework you used to build it.

Stack is still new but it is growing. Check out the list of community [Stack middlewares][5] to see how you can start painlessly adding new features to your Syfmony HTTP Kernel based application.

{% endblock %}

{% block project_cta %}

Do you think your business could be made simpler by leveraging Stack? [Contact us]({{site.url}}/contact/) to see what ideas we have for how Stack can improve your business.

{% endblock %}

[1]: {{site.url}}/projects/hawk/
[2]: {{site.url}}/projects/stack-hawk/
[3]: http://stackphp.com/media/
[4]: https://speakerdeck.com/igorw/the-httpkernelinterface-is-a-lie
[5]: http://stackphp.com/middlewares/
