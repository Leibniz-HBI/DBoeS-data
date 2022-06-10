# Datenbank öffentlicher Sprecher

*Abstract:* The Datenbank öffentlicher Sprecher (Database of Public Speakers, DBöS) is a data collection and curation project at the Leibniz Institute for Media Resesarch | Hans-Bredow-Institut that aims to contain i.a. all the names of parliamentarians in Germany with their party affiliation and their URLs to online social networks (if available). Our first goal is a minimum viable product ([MVP](https://en.wikipedia.org/wiki/Minimum_viable_product)) to keep this part of the database up to date with names and party affiliations. Other attributes, such as gender or age, introduce further complications and will be added later on a per project need’s basis. 

There are 16 federal states and every one has its own local parliament. Additionally to the local parliamentarian politicians the aim is to add all the politicians that are a member of the Bundestag (The Federal Parliament) and the members of the state governments in order to include all members of the Bundesrat (Federal Council). Each of these parliaments gets elected at different points in time. This adds up to a number of around 2700 names from different parties around Germany that have to be kept up to date several times a year.

Therefore, the objective of this concept is to automate the process of keeping the list updated as far as possible. The scraper part supports a researcher/programme with automating data retrieval/search from different platforms. The editor part is such a programme making use of the scraper. It's a Shiny application that helps researchers and assistants to keep the data up to date. The db is basically a 'database', for simplicity's and sustainable archival's sake consisting of plain CSVs.

This repository contains versioned data that is used in the repository https://github.com/Leibniz-HBI/DBoeS-Automatization/

Recommended R Import (setting colClasses prevents corruption of large number IDs):
```
dboes_data <- read.csv("BT-Wahl 2021 Kandidierende.csv", colClasses = "character", encoding = "UTF-8")
```

## Updates
* Release 2021-09-25: 
  * Parlamentarier.csv: Bundestagsabgeordnete am Ende der 19. Legislaturperiode sowie die Landtagsabgeordneten, ein Tag vor der Wahl zum 20. Deutschen Bundestag, und den Landtagswahlen in Berlin und M-V am 26.09.2021
  * BT-Wahl 2021 Kandidierende.csv: Alle Kandierenden zur Bundestagswahl 2021
  * Parteigliederungen.csv: Bundes- und Landesverbände, Fraktionen und Jugendorganisationen aller im Bundestag sowie in Landtagen vertretenen Parteien

---

This data collection is part of the [Social Media Observatory of the Lebniz Institut of Media research | Hans Bredow Institut](https://leibniz-hbi.github.io/SMO/) 
