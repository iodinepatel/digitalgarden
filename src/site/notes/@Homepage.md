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


| File                            |
| ------------------------------- |
| [[@Atomic\|@Atomic]]         |
| [[@Dictionary\|@Dictionary]] |
| [[@Project\|@Project]]       |
| [[@Foundation\|@Foundation]] |
| [[@Level1\|@Level1]]         |
| [[@Finance\|@Finance]]       |
| [[@Language\|@Language]]     |
| [[@Philosophy\|@Philosophy]] |
| [[@Anecdote\|@Anecdote]]     |
| [[@Article\|@Article]]       |
| [[@Audio\|@Audio]]           |
| [[@Book\|@Book]]             |
| [[@Course\|@Course]]         |
| [[@Humour\|@Humour]]         |
| [[@Lines\|@Lines]]           |
| [[@Paper\|@Paper]]           |
| [[@People\|@People]]         |
| [[@Podcast\|@Podcast]]       |
| [[@Poetry\|@Poetry]]         |
| [[@Post\|@Post]]             |
| [[@Quote\|@Quote]]           |
| [[@Visual\|@Visual]]         |
| [[@Website\|@Website]]       |
| [[@Config\|@Config]]         |
| [[@Draft\|@Draft]]           |
| [[@Flora\|@Flora]]           |
| [[@Journal\|@Journal]]       |
| [[@Recipe\|@Recipe]]         |

{ .block-language-dataview}