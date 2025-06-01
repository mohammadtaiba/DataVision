# Checkliste für Visualisierungen

## In `btc_technical_analysis.ipynb`
- [ ] Streudiagramm: RSI vs. Bitcoin-Schlusskurs
- [ ] Streudiagramm: MACD vs. gleitendem Durchschnitt (MA_20) im Verhältnis zum Bitcoin-Schlusskurs
- [ ] Kombinierter Boxplot: Verteilungen von RSI, MACD und Handelsvolumen (zur Identifikation von Ausreißern)
- [ ] Boxplot: Handelsvolumen nach Trendline-Kategorie (aufsteigend / absteigend / seitwärts)
- [ ] Hexagonales Binning: Bitcoin-Schlusskurs vs. Handelsvolumen zur Darstellung dichter Bereiche

## In `btc_vs_gold.ipynb`
- [ ] Streudiagramm: Bitcoin-Schlusskurs vs. Gold-Schlusskurs (gleiche Tage)
- [ ] Boxplot: Tägliche Renditen von Bitcoin (ret_btc) und Gold (ret_xau) im Vergleich
- [ ] Hexagonales Binning: Tägliche Rendite von Bitcoin vs. tägliche Rendite von Gold

---

# Checkliste für Analysen

* [ ] **Analysen durchführen**:
  * [ ] Korrelationen:
    * [ ] RSI, MACD und MA_20 im Vergleich zum Bitcoin-Schlusskurs (`btc_technical_analysis.ipynb`)
    * [ ] Bitcoin-Schlusskurs im Vergleich zum Gold-Schlusskurs (`btc_vs_gold.ipynb`)
  * [ ] Kontingenz-/Kreuztabellen:
    * [ ] Preislevel vs. Handelssignal oder Trendlinie (`btc_technical_analysis.ipynb`)
