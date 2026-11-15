---
title: "Regionen"
permalink: /mc-regionen
---

Regionen halten Nachrichten dort, wo sie hingehören. Ohne Region-Scope leiten alle Repeater alles
weiter, und das Netz läuft voll.

Der Raum Heilbronn gehört zur Region von [THE MÄSH](https://the-maesh.de/) (`de-bw-str`). Eine
eigene MeshCore-Region für Heilbronn melden wir bewusst nicht an.

| Region | Gebiet |
|---|---|
| `#de-bw-hn` | Landkreis Heilbronn |
| `#de-bw-sha` | Schwäbisch Hall (Nachbar) |
| `#de-bw-str` | Metropolregion Stuttgart, THE MÄSH |
| `#de-bw` | Baden-Württemberg |
| `#de-sued` | Süddeutschland |
| `#de` | Deutschland |
| `#europe` | Europa |

Die vollständige Liste mit allen Landkreisen steht bei
[THE MÄSH](https://the-maesh.de/repeater/).

## Eingabe am Companion

In der MeshCore-App pro Kanal den Region-Scope eintragen, ohne `#`, z. B. `de-bw-str` für
`#test-bw-str` (siehe [Client](/mc-client)).

## Eingabe am Repeater

Über die Kommandozeile des Repeaters (USB-Konsole oder Fernverwaltung in der App), ab Firmware
1.10. Beispiel für einen Repeater im Landkreis Heilbronn:

```
region put #de-bw
region put #de-bw-str
region put #de-bw-hn
region home #de-bw-hn
region default #de-bw-str
region save
```

| Befehl | Wirkung |
|---|---|
| `region put <name> [eltern]` | Region anlegen, optional unter einer Elternregion |
| `region home <name>` | Heimatregion des Repeaters |
| `region default <name>` | Standard-Scope für die eigenen Adverts (`#de-bw-str`, für ganz BaWü `#de-bw`) |
| `region save` | Änderungen dauerhaft speichern, sonst sind sie nach dem Neustart weg |
| `region` | alle Regionen und ihre Flood-Rechte anzeigen |
| `region remove <name>` | Region löschen (vorher ihre Unterregionen) |

An Kreisgrenzen zusätzlich die Nachbarregion anlegen, z. B. `region put #de-bw-sha`.

Alle Befehle: [MeshCore CLI-Referenz](https://github.com/meshcore-dev/MeshCore/blob/main/docs/cli_commands.md#region-management-v110).

Stand 2026-11-15.
