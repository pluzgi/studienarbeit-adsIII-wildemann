# Studienarbeit- ADS III - Die Stimme des Widerstands: Eine Analyse der Medienresonanz auf die Protestaktionen der Letzten Generation

Dieses Projekt analysiert die Medien-Berichterstattung über die Bewegung "Letzte Generation" für den Zeitraum 2021-2023. Ziel ist es, Einblicke in die Medienresonanz und öffentliche Wahrnehmung der Bewegung zu gewinnen. Die Medienberichte wurden von der Webseite des Aktionsbündnisses extrahiert (https://letztegeneration.org/presse/berichterstattung-1/).

## Funktionen
Datensammlung: Scrapen von Artikeln von der Webseite der "Letzten Generation" und Speichern in einer SQLite-Datenbank.

Datenbereinigung: Entfernen von HTML-Tags und Erstellen einer bereinigten CSV.

Datenanalyse: Durchführen von Sentiment-Analysen, Erstellen von Profiling-Reports und Analyse der Artikelverteilung.

Visualisierung: Erstellen von Diagrammen zur Darstellung der Analyseergebnisse.

## Technologien

Sprache: Python

Bibliotheken: BeautifulSoup, pandas, numpy, matplotlib, seaborn, nltk, requests, sqlite3, sweetviz, tqdm, transformers, tensorflow.

Datenbank: SQLite

Visualisierung: Matplotlib, Seaborn, Sweetviz

## Installation
Klonen Sie das Repository:
```
git clone https://github.com/pluzgi/studienarbeit-adsIII-wildemann
```

Installieren Sie die erforderlichen Pakete:
```
$ ./setup.sh
$ pip install -r requirements.txt
```

## Struktur des Projekts
main.ipynb: Jupyter Notebook für das Scraping und die Analyse

requirements.txt: Liste der benötigten Python-Pakete

output/: Verzeichnis für die gespeicherten Analyseergebnisse und Visualisierungen

input/: Verzeichnis für die Eingabedaten und 

WICHTIG: Es gibt im Rahmen der Datenverarbeitung zwei Datenbanken, die aufeinander aufbauen. Die erste, die beim Scrapen erstellt wird, wird als .csv ausgegeben und die Daten wurden in Tableau Prep bereinigt und normalisiert. Mit den Daten aus dieser aktualisierten Datenbank wurde dann ab dem Load-Schritt weitergearbeitet:
data/: Datensatz nach Bereinigung in Tableau Prep
