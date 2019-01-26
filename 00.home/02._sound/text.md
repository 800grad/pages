---
title: kollektiv
creator: benjaminwunn
content:
    items:
        '@page': '/blog'
---

{% set banner = page.media.images|first %}
[intro
headline="WHY NOT HAVE SOME RAVE TO GO?"
banner="{{ banner.url }}"]Bei den vielen [[fa icon=fa-calendar-alt /] CLUB- UND OUTDOOR EVENTS](/events) die wir als Rave Crew veranstalten entstehen regelmässig Audiomitschnitte die wir natürlich nicht für uns behalten wollen. Sie sind sowohl auf [[fa icon=fa-mixcloud /] mixcloud](https://www.mixcloud.com/iloveucrew/) als auch in der Rubrik [[fa icon=fa-compact-disc /] Sound](/sound) zu hören.

**DANCE LIKE NO ONE IS WATCHING**[/intro]


<div class="cards">
    {% for image in page.find('/audio').media.images|reverse|slice(0, 3)%}
    <div class="card">
        <a href="{{image.cloudcasturl}}">
        <figure class="cardimage">
            <img data-src="{{image.url}}" class="unveil">
            <figcaption>{{image.mixname}}</figcation>
        </figure>
        </a>
    </div>
    {% endfor %}
</div>

<footer>
<a class="btn" href="/audio">[fa icon=fa-compact-disc /] Sound</a>
</footer>