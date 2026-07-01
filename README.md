# DataVision - Bitcoin vs. Gold Analyse

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerics-013243?logo=numpy&logoColor=white)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-Statistics-blue)
![Prophet](https://img.shields.io/badge/Prophet-Forecasting-black)

DataVision ist ein Data-Science-Projekt zur vergleichenden Analyse von Bitcoin (BTC/USD) und Gold (XAU/USD). Das Projekt untersucht Preisentwicklung, Volatilität, technische Indikatoren, statistische Zusammenhänge und Prognosemodelle auf Basis historischer Tagesdaten.

## Inhaltsverzeichnis

- [Projektziel](#projektziel)
- [Aktueller Status](#aktueller-status)
- [Screenshots und Ergebnisse](#screenshots-und-ergebnisse)
- [Features](#features)
- [Tech-Stack](#tech-stack)
- [Installation und lokaler Start](#installation-und-lokaler-start)
- [Nutzung](#nutzung)
- [Tests](#tests)
- [Projektstruktur](#projektstruktur)
- [License](#License)

## Projektziel

Ziel des Projekts ist es, das Marktverhalten von Bitcoin und Gold datenbasiert zu vergleichen. Im Fokus stehen:

- Analyse der Preisentwicklung von BTC/USD und XAU/USD
- Vergleich der Volatilität beider Anlageklassen
- Untersuchung technischer Indikatoren wie RSI, MACD und gleitender Durchschnitte
- Bewertung statistischer Zusammenhänge mit Hypothesentests
- Modellierung von Marktphasen und Preisprognosen
- Visualisierung zentraler Muster, Ausreißer und Korrelationen

Die Analyse orientiert sich am CRISP-DM-Prozess mit den Phasen Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation und Deployment.

## Aktueller Status

| Bereich | Status |
| --- | --- |
| Datenanalyse | Abgeschlossen |
| Datenbereinigung | Abgeschlossen |
| Technische Indikatoren | Abgeschlossen |
| Visualisierungen | Abgeschlossen |
| Hypothesentests | Abgeschlossen |
| Regression und Klassifikation | Abgeschlossen |
| Prophet-Prognose | Abgeschlossen |
| Automatisierte Tests | Nicht dokumentiert |

Die wichtigsten Ergebnisse zeigen, dass Bitcoin im Vergleich zu Gold deutlich stärkere Preisschwankungen aufweist. Gold zeigt stabilere Preiscluster, während Bitcoin durch hohe Streuung, starke Ausreißer und dynamischere Trendbewegungen geprägt ist.

## Screenshots und Ergebnisse

Die folgenden Abbildungen wurden aus der Projektdokumentation extrahiert und im Ordner `docs/screenshots` abgelegt.

### 1. Schlusskurse von Bitcoin und Gold

<img src="docs/screenshots/01-schlusskurse-btc-xau-logarithmisch.png" alt="Täglicher Verlauf der Schlusskurse von BTC und XAU" width="800">

Der logarithmische Kursverlauf zeigt die langfristige Entwicklung beider Anlageklassen. Bitcoin weist deutlich stärkere Wachstums- und Korrekturphasen auf, während Gold stabiler verläuft.

### 2. Histogramme der Preise und technischen Indikatoren

<img src="docs/screenshots/02-histogramme-preise-indikatoren.png" alt="Histogramme von Preisen und technischen Indikatoren" width="800">

Die Verteilungen zeigen große Unterschiede zwischen BTC und XAU. Bitcoin besitzt breitere Streuungen und stärkere Ausreißer, während Gold klarere Preisbereiche und stabilere technische Werte zeigt.

### 3. BTC-Schlusskurs vs. XAU-Schlusskurs

<img src="docs/screenshots/03-streudiagramm-btc-xau-schlusskurse.png" alt="Streudiagramm BTC-Schlusskurs vs. XAU-Schlusskurs" width="800">

Das Streudiagramm visualisiert den Zusammenhang zwischen Bitcoin- und Goldpreisen über verschiedene Jahre. Es zeigt zeitliche Cluster und eine erkennbare langfristige Mitbewegung.

### 4. Technische Indikatoren und Handelsvolumen

<img src="docs/screenshots/04-streudiagramme-indikatoren-volumen.png" alt="Streudiagramme zu RSI, MACD und MA20 mit Handelsvolumen" width="800">

Die Streudiagramme vergleichen RSI, MACD und MA20 mit den jeweiligen Preisen. Besonders der gleitende Durchschnitt zeigt einen starken Zusammenhang mit dem Preisverlauf.

### 5. Tägliche Renditen

<img src="docs/screenshots/05-boxplot-taegliche-renditen.png" alt="Boxplot der täglichen Renditen von BTC und XAU" width="800">

Der Boxplot macht sichtbar, dass Bitcoin deutlich größere Renditeschwankungen und mehr Ausreißer besitzt als Gold.

### 6. Hexagonales Binning der Renditen

<img src="docs/screenshots/06-hexbin-taegliche-renditen.png" alt="Hexagonales Binning der täglichen Renditen" width="700">

Das Hexbin-Diagramm zeigt die gemeinsame Verteilung der täglichen Renditen. Die meisten Beobachtungen liegen nahe null, einzelne extreme BTC-Bewegungen treten jedoch stärker hervor.

### 7. Korrelation der Schlusskurse

<img src="docs/screenshots/07-hexbin-korrelation-schlusskurse.png" alt="Hexagonales Binning zur Korrelation der Schlusskurse" width="700">

Die Darstellung zeigt eine positive Korrelation zwischen den Schlusskursen von BTC und XAU. Der Zusammenhang ist sichtbar, aber durch unterschiedliche Dynamiken beider Märkte geprägt.

### 8. Korrelationsmatrix

<img src="docs/screenshots/08-korrelationsmatrix-btc-xau.png" alt="Korrelationsmatrix für BTC, XAU und Cross-Korrelationen" width="800">

Die Heatmaps zeigen interne Korrelationen innerhalb beider Assets sowie Cross-Korrelationen zwischen Bitcoin- und Goldvariablen. Preisnahe Indikatoren korrelieren erwartungsgemäß besonders stark mit den Schlusskursen.

### 9. Gemeinsame Kursbewegungen

<img src="docs/screenshots/09-kontingenztabelle-up-down.png" alt="Kontingenztabelle für gemeinsame Kursbewegungen" width="700">

Die Kontingenztabelle zeigt, wie häufig Bitcoin und Gold gemeinsam steigen oder fallen. Daraus lässt sich ein statistischer Zusammenhang im Up/Down-Verhalten ableiten.

### 10. Preisbereiche von BTC und XAU

<img src="docs/screenshots/10-heatmap-preisbereiche.png" alt="Heatmap der BTC- und XAU-Preisbereiche" width="800">

Die Heatmap gruppiert Preisbereiche beider Assets und zeigt, welche Kombinationen historisch besonders häufig gemeinsam aufgetreten sind.

### 11. Volatilität von BTC und XAU

<img src="docs/screenshots/11-dichteverteilung-volatilitaet.png" alt="Dichteverteilung der absoluten täglichen Renditen" width="700">

Die Dichteverteilung der absoluten Renditen bestätigt, dass Bitcoin volatiler ist als Gold. Die Verteilung von BTC ist breiter und besitzt stärkere Ausschläge.

### 12. Zwei-Weg-ANOVA

<img src="docs/screenshots/12-anova-ergebnis-asset-jahr.png" alt="Ergebnis der Zwei-Weg-ANOVA" width="800">

Die ANOVA untersucht, ob Asset-Typ und Jahr einen signifikanten Einfluss auf die Rendite haben. Die Ergebnisse zeigen signifikante Effekte für Asset und Jahr.

### 13. Monats-ANOVA mit Bootstrap

<img src="docs/screenshots/13-anova-bootstrap-monatsrenditen.png" alt="Bootstrap-F-Werte der Monats-ANOVA" width="800">

Die Bootstrap-Verteilung der F-Werte bewertet, ob sich durchschnittliche BTC-Monatsrenditen signifikant unterscheiden. Das Ergebnis zeigt keinen starken Monatsunterschied.

### 14. BTC-Preis nach Gold-Handelsvolumen

<img src="docs/screenshots/14-anova-gold-volumen-btc-preis.png" alt="BTC-Preis nach Gold-Handelsvolumen" width="800">

Die Gruppierung nach Gold-Handelsvolumen zeigt deutliche Unterschiede im BTC-Preis zwischen niedrigen, mittleren und hohen Volumengruppen.

### 15. Chi-Quadrat-Test

<img src="docs/screenshots/15-chi-quadrat-bootstrap.png" alt="Bootstrap-Chi-Quadrat-Statistik" width="800">

Der Chi-Quadrat-Test prüft den Zusammenhang zwischen BTC- und XAU-Kursbewegungen. Die beobachtete Statistik liegt deutlich außerhalb der typischen Bootstrap-Verteilung.

### 16. Multiple lineare Regression

<img src="docs/screenshots/16-mlr-modellergebnisse.png" alt="Modellergebnisse der multiplen linearen Regression" width="800">

Die Regression nutzt technische Indikatoren von BTC und XAU, um den BTC-Schlusskurs zu erklären. Das Modell erreicht eine hohe Anpassungsgüte.

### 17. Vergleich tatsächlicher und vorhergesagter BTC-Preise

<img src="docs/screenshots/17-mlr-vorhersagevergleich.png" alt="Vergleich tatsächlicher und vorhergesagter BTC-Preise" width="800">

Der Vergleich zeigt, dass die Regression den tatsächlichen BTC-Preisverlauf weitgehend nachvollzieht. Abweichungen werden vor allem in dynamischen Marktphasen sichtbar.

### 18. Klassifikation mit Naive Bayes und LDA

<img src="docs/screenshots/18-klassifikation-naive-bayes-lda.png" alt="Classification Report für Naive Bayes und LDA" width="800">

Die Klassifikation ordnet Marktphasen in `bull`, `bear` und `sideways` ein. LDA erzielt im Vergleich zu Naive Bayes eine etwas höhere Gesamtgenauigkeit.

### 19. Prophet-Prognose für Bitcoin und Gold

<img src="docs/screenshots/19-prophet-vorhersage-btc-gold.png" alt="Prophet-Vorhersage für BTC und Gold" width="800">

Die Prophet-Prognose zeigt historische und prognostizierte Werte für BTC und Gold. Beide Zeitreihen werden gemeinsam visualisiert, um Trends und erwartete Entwicklungen vergleichbar zu machen.

## Features

- Einlesen und Bereinigen historischer BTC- und XAU-Tagesdaten
- Standardisierung von Spaltennamen und Datumsformaten
- Berechnung technischer Indikatoren:
    - RSI
    - MACD
    - gleitender Durchschnitt über 20 Tage
    - Trendlinienindikator
- Zusammenführung beider Datensätze über gemeinsame Tagesdaten
- Deskriptive Statistik mit Konfidenzintervallen
- Visualisierung von Kursverläufen, Renditen, Korrelationen und Preisbereichen
- Hypothesentests mit Bootstrap-Sampling
- Multiple lineare Regression zur Preisprognose
- Klassifikation von Marktphasen mit Naive Bayes und LDA
- Zeitreihenprognose mit Prophet

## Tech-Stack

| Kategorie | Technologien |
| --- | --- |
| Sprache | Python |
| Analyse | Pandas, NumPy |
| Visualisierung | Matplotlib, Seaborn |
| Statistik | SciPy, Statsmodels |
| Machine Learning | Scikit-learn |
| Forecasting | Prophet |
| Umgebung | Jupyter Notebook |
| Datenformat | CSV |

## Installation und lokaler Start

```bash
git clone https://github.com/mohammadtaiba/DataVision
cd DataVision
```

```bash
python -m venv .venv
source .venv/bin/activate
```

Für Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Abhängigkeiten installieren:

```bash
pip install -r requirements.txt
```

Jupyter Notebook starten:

```bash
jupyter notebook
```

## Nutzung

Die Analyse erwartet historische Tagesdaten für Bitcoin und Gold. Die im Projekt verwendeten Dateien sind:

```text
BTCUSD_1d_analysis.csv
XAUUSD_1d_analysis.csv
```

Beispiel zum Laden des finalen Datensatzes:

```python
import pandas as pd

final_dataset = pd.read_csv("data/final_merged_dataset.csv", parse_dates=["date"])
print(final_dataset.head())
```

Beispiel für eine einfache Renditeberechnung:

```python
final_dataset["ret_btc"] = final_dataset["close_btc"].pct_change()
final_dataset["ret_xau"] = final_dataset["close_xau"].pct_change()
```

## Tests

Automatisierte Tests sind aktuell nicht dokumentiert. Für eine reproduzierbare Prüfung sollte das Notebook vollständig ausgeführt werden:

```bash
jupyter notebook
```

Empfohlene manuelle Prüfungen:

- Alle Datenquellen lassen sich ohne Fehler laden.
- Der finale zusammengeführte Datensatz enthält keine fehlenden Kernwerte.
- Alle Visualisierungen werden erzeugt.
- Alle Modell- und Testzellen laufen ohne Fehler durch.

## Projektstruktur

Aktuelle Struktur des Repositorys:

```text
.
├── data-vision-site/  # MkDocs-Seite mit aufbereiteten Projektdokumenten
├── dataset/           # Eingabe- und Ausgabedaten der Analyse
├── docs/              # Screenshots und ergänzende Dokumentation
├── notebooks/         # Jupyter-Notebooks für Datenanalyse und Visualisierung
├── .gitignore         # Git-Ignorierregeln für lokale und generierte Dateien
├── LICENSE            # Lizenzinformationen
├── README.md          # Projektübersicht und Einstiegspunkt
└── requirements.txt   # Python-Abhängigkeiten für den lokalen Start
```

## License

Copyright (c) 2026 Mohammad Taiba. All rights reserved.

This project is published for portfolio and review purposes only. See [LICENSE](./LICENSE).
