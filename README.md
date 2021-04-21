# Daten aus dem SARS-CoV-2 Contact Tracing im Kanton Zürich

<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>
<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19_contact_tracing_ZH/commits/master)

**Die Gesundheitsdirektion Kanton Zürich veröffentlicht im Rahmen des kantonalen Contact Tracings erhobene Daten zum Ansteckungskontext SARS-CoV-2-positiv getesteter Personen im Kanton Zürich. Die Daten 2020 wurden mit einem anderen Instrument erhoben als die Daten 2021. Die Daten 2020 und 2021 sind darum nur bedingt vergleichbar.**

# Definitionen
- Als «eindeutig» gilt ein Ansteckungskontext, wenn die befragte Person mit grosser Sicherheit sagen kann, bei wem sie sich angesteckt hat resp. weiss, dass sie in Kontakt mit einer positiv getesteten Person war.

- Als «vermutet» gilt ein Ansteckungskontext, wenn die befragte Person eine konkrete Vermutung über den Ansteckungsweg hat. Diese wird in einem strukturierten Gespräch erörtert, bleibt jedoch subjektiv und ist ensprechend vorsichtig zu interpretieren.

- Als "nicht befragt" werden positiv getestete Personen ausgewiesen, die telefonisch nicht erreicht werden konnten. Gründe dafür sind (fehlende Telefonnummer, unkooperatives Verhalten, Personen in Alters-/Pflegeheimen)

- 2020 wurden nur eindeutige Ansteckungswege nach dem Ansteckungskontext differenziert (Eigener Haushalt, Arbeitsplatz, usw.). 

- Ob eine Ansteckung als eindeutig klassifiziert wird, hängt stark vom Kontext ab. Beispiel: Eine Ansteckung im eigenen Haushalt wird viel eher als eindeutig klassifiziert als eine Ansteckung beim Sport im Freien. Die Daten sind darum verzerrt. Einfach ermittelbare Ansteckungswege sind überdurchschnittlich vertreten. Ein Vergleich der Ansteckungskontexte ist darum nur sehr bedingt möglich. Möglich sind jedoch Aussagen über die zeitliche Entwicklung einzelner Kategorien.

- Die Interpretation der Daten soll folglich zurückhaltend erfolgen, da ein grosser Spielraum für Fehlinterpretationen besteht.



# Bei Fragen

Wir stellen die Daten im Auftrag der [Gesundheitsdirektion des Kantons Zürich](https://www.zh.ch/de/gesundheit/coronavirus.html) zur freien Wiederverwendung zur Verfügung. 

Für inhaltliche Fragen wenden Sie sich bitte an die Gesundheitsddirektion:
gdstab@gd.zh.ch

Für Fragen zur Bereitstellung der Daten erreichen Sie die [Fach- und Koordinationsstelle OGD](https://www.zh.ch/de/politik-staat/opendata.html?keyword=ogd#/home) unter:
- https://twitter.com/OpenDataZH (follow us, we send you a private Direct Message, thanks!)
- info@open.zh.ch

# Datenaktualisierung

Diese Daten werden wöchentlich am Dienstag bis 16:00 Uhr jeweils für die Vorwoche aktualisiert.

# Datenstruktur

## Für Ansteckungswege.csv

| __Field Name__          | __Description__                                | __Format__     |
|---------------------|--------------------------------------------|------------|
| __from__              | Anfangsdatum des ausgewerteten Zeitraums | YYYY-MM-DD |
| __until__              | Enddatum des ausgewerteten Zeitraums | YYYY-MM-DD |
| __context_bool__ | Ansteckungsweg ist eindeutig / vermutet / nicht erhoben | Text |
| __context_cat__     | Ansteckungskontext Kategorie | Text |
| __n_conf__       | Anzahl Fälle | Number |
| __perc_conf__       | Anteil der Kategorie am Total aller Fälle  | Number |
 
