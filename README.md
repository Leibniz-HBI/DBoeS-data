# Datenbank öffentlicher Sprecher (DBÖS)

## Beschreibung

Ziel der „Datenbank öffentlicher Sprecher“ (DBÖS) ist, eine möglichst umfassende und regelmäßig aktualisierte Übersicht von Akteur:innen zu führen, die zu gesellschaftlicher Öffentlichkeit in Deutschland beitragen – im Sinne der die Öffentlichkeit tragenden Medien genauso wie als Sprecher:innen, die in der Öffentlichkeit stehen, oder als Gegenstand öffentlicher Berichterstattung.

Eine ausführliche Beschreibung ihrer Daten findet sich in [DOCUMENTATION.pdf](DOCUMENTATION.pdf).

## Nutzung

Eine Nutzung ist unter Beachtung der [CC-BY Lizenz](LICENSE) jederzeit möglich. Bei akademischen Veröffentlichungen, die sich die Daten zunutze machen bitten wir um eine [Zitation](CITATION).

Die Dateien befinden sich im Ordner '[data](data/)'. Die CSV-Dateien sind entsprechend der in der [Dokumentation](DOCUMENTATION.pdf) beschriebenen Kategorien numeriert. Zudem findet sich darin auch eine XSLX-Datei mit allen Daten für den Gebrauch in Spreadsheet-Editoren wie Libre-Office oder Excel.

---

## Instructions for Contributors

### Update Instructions

#### Setup

Assuming a working [Pipenv installation](https://pipenv.pypa.io/en/latest/installation/), run the following commands in a bash-like shell (please report issues if they arise in other environments):

```bash
pipenv install
pipenv shell
jupyter-lab
```

#### Update data

With a prepared XSLX file containing category-wise sheets named by category-number,
open the notebook `upload.ipynb` in the opening browser interface and follow its instructions.
