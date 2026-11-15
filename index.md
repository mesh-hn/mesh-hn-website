---
layout: splash
title: "MeshCore im Raum Heilbronn"
permalink: /
header:
  overlay_color: "#0b3d2e"
  actions:
    - label: "So stellst du ein"
      url: /mc-client
    - label: "Leute finden"
      url: /mc-webring
excerpt: "Funk-Mesh ohne Internet: Kurznachrichten über LoRa, solarversorgte Repeater, offene Software."
feature_row:
  - title: "Client"
    excerpt: "Dein Gerät (Companion) einrichten: Preset, Kanäle, Region."
    url: /mc-client
    btn_label: "Mehr"
    btn_class: "btn--primary"
  - title: "Repeater"
    excerpt: "Empfohlene Einstellungen und Checkliste für einen Repeater."
    url: /mc-repeater
    btn_label: "Mehr"
    btn_class: "btn--primary"
  - title: "Regionen"
    excerpt: "Welche Regionen im Raum Heilbronn gelten."
    url: /mc-regionen
    btn_label: "Mehr"
    btn_class: "btn--primary"
  - title: "Roomserver"
    excerpt: "Roomserver im Raum Heilbronn."
    url: /mc-roomserver
    btn_label: "Mehr"
    btn_class: "btn--primary"
  - title: "Sensor"
    excerpt: "Sensor-Knoten im Raum Heilbronn."
    url: /mc-sensor
    btn_label: "Mehr"
    btn_class: "btn--primary"
  - title: "Sonstiges"
    excerpt: "Werkzeuge, Karten und andere Mesh-Netze."
    url: /mc-sonstiges
    btn_label: "Mehr"
    btn_class: "btn--primary"
---

## Auf einen Blick

| | |
|---|---|
| Preset | EU/UK Narrow |
| Region (Landkreis Heilbronn) | `#de-bw-hn` |
| Region (Metropolregion Stuttgart) | `#de-bw-str` |
| Repeater-Firmware | mindestens 1.14.0 |

Wir sind die lokale Ebene unter [THE MÄSH](https://the-maesh.de/), der MeshCore-Community der
Metropolregion Stuttgart, zu der Heilbronn-Franken gehört. Die Einstellungen oben stammen von dort.

{% include feature_row %}

## Neuigkeiten

{% for post in site.posts limit:5 %}
- {{ post.date | date: "%d.%m.%Y" }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

[Alle Neuigkeiten](/neuigkeiten/)
