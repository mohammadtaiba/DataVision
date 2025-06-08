# DataVision

---

## 📊 Projektbeschreibung
Dieses Projekt verwendet zwei Finanzdatensätze (Bitcoin-Preisdaten, Gold-Preisdaten), um verschiedene Methoden der Data Science zu demonstrieren:

1. **Bitcoin Price History** – Analyse des Preisverlaufs und der Volatilität von Bitcoin
2. **Gold Price History** – Untersuchung der Preisentwicklung und Stabilität von Gold

Im Fokus steht der Vergleich beider Anlageklassen anhand von statistischen Kennzahlen, Visualisierungen und Hypothesentests.
Zusätzlich wird die Datensätze mit verschiedenen technischen Indikatoren erweitert
(z.B. Moving Averages `20`, RSI, MACD, ...), um marktbezogene Muster und Handelssignale zu analysieren.

---

## 🎯 Ziel
Das Ziel ist es, mithilfe des CRISP-DM-Modells datengetriebene Erkenntnisse zu gewinnen:
Das Projekt verfolgt das Ziel, das Preisverhalten und die Volatilität von Bitcoin im Vergleich zu Gold zu analysieren, um Rückschlüsse auf Stabilität, Risiko und Anlageverhalten zu ziehen. Besonderes Augenmerk liegt auf der Wirksamkeit technischer Indikatoren (wie RSI, MACD und Moving Averages), um Markttrends und Handelssignale zu identifizieren.

Dabei sollen mithilfe des CRISP-DM-Modells datengetriebene Erkenntnisse gewonnen werden:
- Deskriptive Analyse
- Analytische Untersuchung
- Statistische Hypothesentests
- Visualisierung von Mustern und Zusammenhängen
- Visualisierung von Mustern, Preisverläufen und technischen Signalen
- Bewertung von Marktverhalten mithilfe technischer Indikatoren

---


## ✅ Erfolgskriterien (Business Success Criteria)

- Es wurde ein signifikanter Unterschied in der Volatilität zwischen Bitcoin und Gold festgestellt.
- Technische Indikatoren (z. B. RSI, MACD) zeigen eine statistisch signifikante Beziehung zur Kursentwicklung.
- Die Analyse identifiziert mindestens drei wiederkehrende technische Signale oder Muster.
- Hypothesentests bestätigen signifikante Unterschiede im Marktverhalten (p < 0.05).
- Es können fundierte Aussagen über die Stabilität und das Investitionsverhalten der beiden Assets getroffen werden.

---

## 🧪 Data Mining Goals

- Quantitative Analyse der Preisvolatilität von Bitcoin und Gold anhand statistischer Kennzahlen (Mittelwert, Standardabweichung, IQR).
- Untersuchung der Korrelation zwischen Preisverläufen und technischen Indikatoren wie RSI, MACD, Bollinger Bands und Moving Averages.
- Anwendung von Hypothesentests (t-Test, ANOVA, Chi²-Test) zur Validierung von Marktverhalten und Mustererkennung.
- Visualisierung von Kursverläufen und technischen Signalen zur Erkennung potenzieller Handelsmuster.
- Identifikation signifikanter technischer Indikatoren, die zur Prognose von Kursentwicklungen beitragen könnten.

---

## 📈 Data Mining Success Criteria

- Statistische Kennzahlen (Mittelwert, Median, Standardabweichung, IQR) wurden korrekt berechnet und interpretiert.
- Konfidenzintervalle für alle vier Kennzahlen wurden erfolgreich bestimmt.
- Drei unterschiedliche Hypothesentests (t-Test, ANOVA, Chi²-Test) wurden mit Bootstrap-Sampling durchgeführt und ausgewertet.
- Es wurden signifikante Korrelationen (|r| > 0.5) zwischen technischen Indikatoren und Kursverlauf festgestellt.
- Alle geplanten Visualisierungen (Streudiagramm, Hex-Binning, Boxplot) wurden erstellt und sinnvoll interpretiert.
- Die Analyse ist vollständig reproduzierbar im Jupyter Notebook dokumentiert.

---

## 🧠 Methoden
Das Projekt folgt den CRISP-DM Phasen:
@@ -24,24 +66,39 @@ Das Projekt folgt den CRISP-DM Phasen:
5. Evaluation
6. Deployment


**Verwendete Techniken umfassen:**
- Statistische Analyse (z. B. Mittelwert, IQR, t-Test, ANOVA)
- Visualisierungen (Streudiagramme, Boxplots, Zeitreihenplots)
- Technische Analyse (Moving Average, RSI, MACD, Bollinger Bands, Supertrend)

---

## 🛠️ Technologien
- Python
- Jupyter Notebook
- Pandas, Matplotlib, Seaborn, Scikit-Learn
- Hugging Face `datasets` API
- Git

---


## 📁 Projektstruktur

| Ordner / Datei     | Beschreibung                           |
|--------------------|----------------------------------------|
| 📂 dataset/        | Enthält die CSV-Datensätze             |
| ├── 📂  input/     | csv-dateien -> importiert     |
| └── 📂  output     | csv-dateien -> bereinigt & vorbereitet |
| 📂 Docomentation/  | Dokomentation                          |
| 📂 notebooks/      | Jupyter Notebooks für Analysen         |
| 📄 .gitignore     | unnötige Dateiein ignorieren           |
| 📄 README.md       | Projektbeschreibung                    |
| 📄 requirements.txt | Liste der Python-Abhängigkeiten        |

---


## 🔖 Lizenz
Dieses Projekt ist unter keiner spezifischen Lizenz veröffentlicht.