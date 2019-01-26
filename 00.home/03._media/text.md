---
title: kollektiv
creator: benjaminwunn
content:
    items:
        '@page': '/blog'
---

{% set banner = page.media.images|first %}

[intro
headline="Elektrisierende Momente"
banner="{{ banner.url }}"]
Zu guten [[fa icon=fa-calendar-alt /] CLUB- UND OUTDOOR EVENTS](/events) gehört neben dem bombastischen [[fa icon=fa-compact-disc /] Sound](/sound)  natürlich auch Deko, Licht und tanzende Massen. Diese Momente werden ab und zu in Bildform festgehalten und dann in der [[fa icon=fa-camera-retro /] Gallery](/gallery) sowie auf [[fa icon=fa-instagram/] instagram](https://www.instagram.com/iloveu.djcrew/)
von euch und mit euch geteilt.

**A PICTURE TELLS MORE THAN A THOUSAND WORDS**[/intro]

<div class="cards">
    {% for image in page.find('/gallery').media.images|reverse|slice(0, 3)%}
    <div class="card">
        <figure class="cardimage">
            <img data-src="{{image.url}}" class="unveil">
        </figure>
    </div>
    {% endfor %}
</div>

<footer>
<a class="btn" href="/gallery">[fa icon=fa-camera-retro /] Gallery</a>
</footer>