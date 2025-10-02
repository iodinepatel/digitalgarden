---
{"dg-publish":true,"permalink":"/homepage/","tags":["gardenEntry"]}
---


```base
filters:
  and:
    - file.hasTag("dashboard")
    - '!file.inFolder("99 Extension/Template")'
formulas:
  Related Note: |
    file.backlinks.filter(!file(value).path.contains("99 Extension/Template")).length
views:
  - type: cards
    name: Dashboard
    order:
      - file.name
      - formula.Related Note
    sort:
      - property: sort
        direction: ASC
    imageAspectRatio: 0.25
    cardSize: 150

```


