# Datenbank öffentlicher Sprecher (DBÖS)

## Beschreibung

Ziel der „Datenbank öffentlicher Sprecher“ (DBÖS) ist, eine möglichst umfassende und regelmäßig aktualisierte Übersicht von Akteur:innen und ihren Web-Präsenzen zu führen, die zu gesellschaftlicher Öffentlichkeit in Deutschland beitragen – im Sinne der die Öffentlichkeit tragenden Medien genauso wie als Sprecher:innen, die in der Öffentlichkeit stehen, oder als Gegenstand öffentlicher Berichterstattung.

Eine ausführliche Beschreibung ihrer Daten findet sich in [DOCUMENTATION.pdf](DOCUMENTATION.pdf).

## Nutzung

Eine Nutzung ist unter Beachtung der [CC-BY Lizenz](LICENSE) jederzeit möglich. Bei akademischen Veröffentlichungen, die sich die Daten zunutze machen, bitten wir um eine [Zitation](CITATION).

	Schmidt, Jan-Hinrik, Lisa Merten, Felix Victor Münch (2024): Die „Datenbank Öffentlicher
	Sprecher“ (DBÖS). v2. Dezember 2024. Online verfügbar: https://doi.org/10.17605/OSF.IO/SK6T5.

Die Dateien befinden sich im Ordner [data](data/). Die CSV-Dateien sind entsprechend der in der [Dokumentation](DOCUMENTATION.pdf) beschriebenen und in [types.csv](types.csv) gelisteten Typen numeriert. Zudem findet sich darin auch XLSX-Dateien mit allen Daten für den Gebrauch in Spreadsheet-Editoren wie Libre-Office oder Excel.

Der DBÖS liegt ein typ- und kategorienübergreifendes Datenmodell zugrunde. Die einzelnen Listen enthalten alle die gleichen Variablen, die in Tab. 20 der [Dokumentation](DOCUMENTATION.pdf) erläutert sind. Variablen mit Angaben zu Social-Media-Profilen haben das Präfix „SM_“, kategorienspezifische Variablen (z.B. das Geschlecht bei Personen) das Präfix „K_“ und typenspezifische Variablen (z.B. das Parlament, in dem ein:e Politiker:in das Mandat hat) besitzen das Präfix „T_“. Je nach Typ sind dadurch manche kategorien- und typenspezifischen Variablen leer. Sie sind dennoch in der Tabellenstruktur enthalten, um verschiedene Listen rasch zusammenfügen zu können.

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

With a prepared XLSX file containing category-wise sheets named by category-number,
open the notebook `upload.ipynb` in the opening browser interface and follow its instructions.
