---
title: "Repeater"
permalink: /mc-repeater
---

Repeater leiten Nachrichten weiter und bilden das Mesh. Bevor du einen aufstellst, prüfe auf der
[Karte](https://str.meshmapper.net/), ob die Gegend schon versorgt ist: Zu viele Repeater machen
das Netz schlechter, nicht besser.

* [Checkliste Repeater](https://docs.google.com/document/d/1PHjF8IdYAYHtn65k7ZsUfaFQFmNKLTME1hTQks-MexA/mobilebasic)

## Empfohlene Einstellungen

- **Firmware** aktuell halten, mindestens 1.14.0 (Regionen und 2-Byte-Pfade).
- **Regionen** einheitlich setzen, siehe [Regionen](/mc-regionen). Als Heimatregion im Landkreis
  Heilbronn `#de-bw-hn`, an Kreisgrenzen zusätzlich die Nachbarregion.
- **Gastzugang** durch ein Passwort abschalten.
- **Adverts** sparsam: Zero-Hop-Adverts auf das Maximum (240 Minuten). Ein Flood-Advert nach dem
  Einrichten oder größeren Änderungen, danach ein langer Abstand, z. B. 150 Stunden.

Diese Werte testen derzeit mehrere Repeater-Admins bei THE MÄSH, eine feste Empfehlung gibt es
noch nicht:

```
set flood.max.unscoped 5
set flood.max 16
set flood.max.advert 16
set path.hash.mode 2
set dutycycle 10
```

`flood.max` begrenzt die Weiterleitungen einer Nachricht: 16 empfohlen, höchstens 20.

Stand 2026-11-15, übernommen von [the-maesh.de](https://the-maesh.de/repeater/).
