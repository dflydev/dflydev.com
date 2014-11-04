---
permalink: madisonphp2014/index.html
title: Madison PHP 2014
header: Your Problems Solved.
---
{% block long_description %}
<style>
.landing-image {
    float: right; max-width: 100px; height: auto; margin: .5em;
}

@media only screen and (max-width: 420px) {
    .ck_embed_form.ck_vertical_subscription_form {
        width: auto;
    }

    .ck_embed_form .ck_embed_form_content {
        padding: 10px;
    }

    .ck_embed_form .ck_subscribe_form {
        padding: 10px;
    }
}
@media only screen and (min-width: 768px) {
    .landing-image {
    }
}
@media only screen and (min-width: 992px) {
    .landing-image {
        float: right; max-width: 150px; height: auto; margin: 1em;
    }
}
</style>

<h1>Attending Madison PHP?</h1>

<a href="http://2014.madisonphpconference.com/"><img class="landing-image" src="{{ site.url }}/assets/landings/madisonphp-logo.png"></a>

<p>
    <strong>We'll be there too!</strong> And we'd <strong>love</strong> to find out more about
    <strong>you</strong>, <strong>your business</strong>, and what <strong>you</strong> want to get out of Madison PHP!
</p>

<p>
    Are you hoping to learn about the hip new tools to start your next project?
    Find out how you can go about modernizing your existing applications? Or are
    you hoping to find new ideas for how you can better grow your business?
</p>

<p>
    We're huge fans of framework agnostic code and Domain-Driven Design (DDD). If
    you'd like to learn more about how following DDD practices and making your
    software framework agnostic can help your business, sign up for our short email
    course on applying these tools to your next project!
</p>
<p>
    PS: Make sure to check out our very own <a href="https://beau.io">Beau Simensen</a>
    presenting <a href="http://2014.madisonphpconference.com/schedule/view/5/namespaces-and-autoloading-beau-simensen">Namespaces and Autoloading</a>
    on the PHP Foundations Track! Track him down at any point if you'd like to chat
    with him about anything!
</p>

<br>

<script src="https://app.convertkit.com/landing_pages/766.js?orient=vert"></script>


{% endblock %}
{% block scripts %}
<script>
(function () {
    if (matchMedia) {
        var $form = $('.ck_embed_form');

        var listener = function (mq) {
            if (mq.matches) {
                $form.removeClass('ck_vertical_subscription_form');
                $form.addClass('ck_horizontal_subscription_form');
            } else {
                $form.addClass('ck_vertical_subscription_form');
                $form.removeClass('ck_horizontal_subscription_form');
            }
        };

        var mq = window.matchMedia("(min-width: 630px)");
        mq.addListener(listener);
        listener(mq);
    }
})();
</script>

{% endblock %}
