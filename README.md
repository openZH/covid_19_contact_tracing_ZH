# Daten aus dem SARS-CoV-2 Contact Tracing im Kanton Zürich

<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>
<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19_contact_tracing_ZH/commits/master)

**Dies ist eine Beta-Version. Wir werden kontinuierlich an der Aufarbeitung und Verbesserung der zur Verfügung stehenden Datengrundlage arbeiten.**

# Definitionen
- Als «nicht eindeutig» gilt ein Ansteckungskontext, wenn die befragte Person nicht weiss, bei wem sie sich angesteckt hat resp. die Frage, ob sie in Kontakt mit einer auf das Coronavirus positiv getesteten Person war, verneint.

- Nur wenn der Ansteckungsweg eindeutig ist, wird nach dem Ansteckungskontext (Eigener Haushalt, Arbeitsplatz, usw.) differenziert. 

- Dass ein Ansteckungskontext als eindeutig klassifiziert wird, ist umso wahrscheinlicher, je klarer andere Personen zu diesem Ansteckungskontext zugeordnet werden können. Beispiel: Eine Ansteckung im eigenen Haushalt wird viel eher als eindeutig klassifiziert als eine Ansteckung beim Sport im Freien.

- Diese Daten erlauben keine Aussage über Ansteckungskontexte von Personen, die nicht eindeutig wissen, bei wem sie sich angesteckt haben.

- Die Interpretation der Daten soll folglich zurückhaltend erfolgen, da ein grosser Spielraum für Fehlinterpretationen besteht.



# Bei Fragen

Wir stellen die Daten im Auftrag der [Gesundheitsdirektion des Kantons Zürich](https://www.zh.ch/de/gesundheit/coronavirus.html) zur freien Wiederverwendung zur Verfügung. 

Für inhaltliche Fragen wenden Sie sich bitte an die Gesundheitsddirektion:
gdstab@gd.zh.ch

Für Fragen zur Bereitstellung der Daten erreichen Sie die [Fach- und Koordinationsstelle OGD](https://www.zh.ch/de/politik-staat/opendata.html?keyword=ogd#/home) unter:
- https://twitter.com/OpenDataZH (follow us, we send you a private Direct Message, thanks!)
- info@open.zh.ch

# Datenaktualisierung

Voraussichtlich werden die Daten alle zwei Wochen aktualisiert werden.


# Datenstruktur

## Für Ansteckungswege.csv

| __Field Name__          | __Description__                                | __Format__     |
|---------------------|--------------------------------------------|------------|
| __from__              | Anfangsdatum des ausgewerteten Zeitraums | YYYY-MM-DD |
| __until__              | Enddatum des ausgewerteten Zeitraums | YYYY-MM-DD |
| __context_bool__ | Ansteckungsweg ist eindeutig / nicht eindeutig | Text |
| __context_cat__     | Ansteckungskontext Kategorie | Text |
| __n_conf__       | Anzahl Fälle | Number |
| __perc_conf__       | Anteil der Kategorie am Total aller Fälle  | Number |

Ohne Angabe beim Ansteckungskontext meint: Bekannte infizierende Person, aber ohne Angabe des Kontexts. 
