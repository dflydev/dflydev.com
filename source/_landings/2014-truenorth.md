---
permalink: tnphp14/index.html
title: True North PHP 2014
header: Your Problems Solved.
---
{% block long_description %}
<style>
.landing-image {
    float: right; max-width: 100px; height: auto; margin: .5em;
}

@media only screen and (min-width: 992px) {
    .landing-image {
        float: right; max-width: 150px; height: auto; margin: 1em;
    }
}
</style>

<h1>Attending True North PHP?</h1>

<p><a href="http://truenorthphp.ca"><img class="landing-image" src="/assets/landings/truenorthphp-logo.png"></a></p>

<p>
We wish we could be there, too! The <a href="http://truenorthphp.ca/schedule.php">schedule</a> this year looks amazing! Unfortunately we'll have to settle for being there in spirit only this year.
</p>

<p>
Even though we cannot be there in person this year we wanted to help at least one other person get there who might not otherwise have been able to attend. Thanks to the True North team we were able to make this happen by becoming a Scholarship Sponsor for True North PHP 2014.
</p>

<p>
We believe that community is powerful and that diversity is important. Sponsoring scholarships for community conferences is a small way that we can give back to the community and to lower at least some of the barriers that may keep people from conferencing.
</p>

<br>

<script src="https://app.convertkit.com/landing_pages/766.js?orient=vert&ref=tnphp14"></script>


{% endblock %}
{% block scripts %}
<script>
(function () {
    return;
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
