---
title: kollektiv
creator: benjaminwunn
content:
    items:
        '@page': '/crew'
---
{% set banner = page.media.images|first %}

[intro
headline="das kollektiv stellt sich vor"
banner="{{ banner.url }}"]
[logo]MTHRFCKN**BASS**[/logo] ist ein [[fa icon=fa-users /] Kollektiv](/crew) von DJs aus dem Rhein-Main Gebiet. Seit 2011 veranstalten wir kostendeckend ausgelegte [[fa icon=fa-calendar-alt /] Club- und Outdoor Events](/events). Unser [[fa icon=fa-compact-disc /] Sound](/sound) ist elektronisch und deckt unter anderem House, Techhouse & Techno ab. Zu den Zielen gehört selbstverwaltetes, gemeinschaftliches Feiern in der frankfurter Umgebung sowie ein [[fa icon=fa-camera-retro /] freundschaftlicher, kollegialer Umgang mit dem Puplikum](/gallery).

**IN DIESEM SINNE: RAVE ON**[/intro]


<!---
[card image="./home/_kollektiv/kaozz.jpg" headline="Kaozz." title="Get MAD" linktarget="/crew/kaozz"]
Techno, Tech-House & UK-Bass
[/card]

[card image="./home/_kollektiv/ostblockangie.jpg" headline="Ostblock Angie" title="Aus dem Herzen Europas" linktarget="/crew/ostblock-angie"]
Techno
[/card]

[card image="./home/_kollektiv/bobbyforward.jpg" headline="Bobby Forward" title="Richard Drauf" linktarget="/crew/bobby-forward"]
Techno, Tech-House & UK-Bass
[/card]
--->

[cards]
{% for p in page.collection %}
{% set cardimage = p.media.images|first %}
[card image="{{ cardimage.url }}" headline="{{ p.title }}" title="{{ p.slogan }}" linktarget="{{ p.url }}"]
{{ p.genre }}
[/card]
{% endfor %}
[/cards]
