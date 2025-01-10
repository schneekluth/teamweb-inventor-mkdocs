---
title: Unsere Hot-Dog Auswahl
description: Unser Sortiment and wohlschmeckenden Hot Dogs
hide:
  #- navigation
  #- toc
search:
  exclude: false
---

# Unser Sortiment

## Hotdogs
!!! info ""
    [Tabellen :octicons-link-external-16:](https://squidfunk.github.io/mkdocs-material/reference/data-tables/) können einfach in Markdown geschrieben und formatiert werden.

    Es besteht auch die Möglichkeit Excel-Dokumente einzulesen, was im Beispiel der [Beilagen](#beilagen) erläutert wird.

| Hot Dog (linkbündig) | Preis (rechtsbündig) | Anmerkung (zentriert)     |
| -------------------- | -------------------: | :-----------------------: |
| Groß                 | 8,50€                | Für den **großen** Hunger |
| Mittel               | 5,25€                | Sehr lecker               |
| Klein                | 3,50€                | Für die kleinen Gäste     |

## Beilagen
Damit man nicht fortlaufend alle Beilagen auf dieser Seite pflegen muss, wurden sie in die Datei `includes/beispiel.xlsx` auf das zweite Blatt mit dem namen `Beilagen` ausgelagert und können mit einem einfachen Kommando automatisch in dieser Webseite eingelesen werden:

Dazu wird der Befehl `read_excel()` benutzt, auf den Ablageort der Datei (relativ zur `mkdocs.yml`) und das entsprechende Blatt im Excel-Dokument verwiesen:
```
read_excel('../includes/beispiel.xlsx', engine='openpyxl', sheet_name="Beilagen")
```

**Das Ergebnis:**

{{ read_excel('../includes/beispiel.xlsx', engine='openpyxl', sheet_name="Beilagen") }}

## Serviervorschlag
### Guacamole
Wer mag keine Guacamole auf seinem Hot Dog? Besser noch, wenn man ein Zubereitungsvideo direkt auf dieser Seite einbinden und darstellen kann:

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/dNJdJIwCF_Y?si=r4l1_E4ac6pSAJiV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</center>

### Käse
<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/Y8F-0Ogp4fU?si=3Zlp1QmADBbS6UJp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</center>
