---
title: "Client (Companion) einrichten"
permalink: /mc-client
---

Ein Companion ist ein kleines LoRa-Gerät, das du per Bluetooth mit Handy, Tablet oder Rechner
verbindest. Companions leiten nichts weiter, das machen die Repeater.

1. MeshCore über den [Webflasher](https://meshcore.io/flasher) auf das Gerät bringen.
2. Die MeshCore-App installieren (Android, iOS, Windows, macOS) und per Bluetooth koppeln.
3. In den Einstellungen das Preset **EU/UK Narrow** wählen und dem Gerät einen Namen geben.
4. Kanäle anlegen und für jeden Kanal einen Region-Scope setzen (siehe [Regionen](/mc-regionen)).

## Kanäle

Diese Kanäle empfiehlt [THE MÄSH](https://the-maesh.de/benutzen/) für die Region, mit Scope:

| Kanal | Scope |
|---|---|
| `#stuttgart` | `de-bw-str` |
| `#test-bw-str` | `de-bw-str` |
| `#test-bw` | `de-bw` |
| `#test`, `#mctechtalk`, `#netzstatus`, `#marktplatz`, `#blackout` | |

Einen eigenen Kanal für den Raum Heilbronn gibt es noch nicht.

Für die erste Nachricht: Kanal `#test-bw-str` mit Scope `de-bw-str` anlegen und etwas schicken.
Unter der Nachricht siehst du, ob und wie oft Repeater in deiner Nähe sie weitergeleitet haben.

Stand 2026-11-15, übernommen von [the-maesh.de](https://the-maesh.de/benutzen/).
