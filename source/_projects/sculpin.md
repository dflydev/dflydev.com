---
permalink: projects/sculpin/
title: Sculpin
is_featured: true
tags:
    - php
logos:
    small: assets/projects/sculpin-mascot-jackson-medium@2x.png
    large: assets/projects/sculpin-mascot-jackson-large@2x.png
website: http://sculpin.io
github: https://github.com/sculpin
twitter: getsculpin

---
{% block short_description %}

An extensible PHP static site generator.

{% endblock %}
{% block long_description %}

> Sculpin is a static site generator written in PHP. It converts Markdown files, Twig templates or standard HTML into a static HTML site that can be easily deployed.

Are you worried that your business site is going to be brought to its knees by unexpectedly going viral? You should be. Unless you have prepared for it well in advance, many sites crumble under the full force of *really* going viral.

This is one of the big reasons that static site generators seem to be all the rate these days. What business wants to be down for *any* reason exactly when they are getting more traffic than they expected?

Static sites are sites where all of the content is generated in advance of being deployed in production. This means that your production environment typically only needs to include a web server. No other tools are required.

In fact, static sites can even be deployed directly to a CDN like [CloudFront](http://aws.amazon.com/cloudfront/) or [CloudFlare](https://www.cloudflare.com/) for ultimate speed and availability. Leave handling traffic bursts to the experts!

If your project doesn't actually need to be dynamically generated on every page load, Sculpin may be your answer. Especially if your team is already comfortable with PHP they will feel right at home with Sculpin.

We wrote Sculpin because we wanted to fix some issues we had with Jekyll. We chose PHP because we are comfortable with it. Since then we've used Sculpin to build literally dozens of sites, [including the one you are visiting now](https://github.com/dflydev/dflydev.com).

Sculpin is a member project of the [PHP Framework Interoperability Group](http://www.php-fig.org/) so you can know that we are serious about making Sculpin a tool that your business can rely on.

{% endblock %}

{% block project_cta %}

Are you worried about whether your site can handle going viral? Do you think that going static might be an option? Not sure? [Contact us]({{site.url}}/contact/) for a <strong>free 30 minute consultation</strong> to see if going static makes sense for your business.

{% endblock %}
