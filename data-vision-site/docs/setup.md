# 📦 Setup & Build-Befehle

## 🔹 Voraussetzungen installieren

pip install mkdocs mkdocs-material


## 🔹 Lokale Vorschau starten

 - cd data-vision-site
 - mkdocs serve
 

---

## 🔹 HTML-Seiten (ohne Input-Zellen) generieren

 
 - jupyter nbconvert notebooks/btc.ipynb --to html --no-input --output-dir=data-vision-site/docs/notebooks --output=btc.html
 - jupyter nbconvert notebooks/xau.ipynb --to html --no-input --output-dir=data-vision-site/docs/notebooks --output=xau.html
 - jupyter nbconvert notebooks/indicators.ipynb --to html --no-input --output-dir=data-vision-site/docs/notebooks --output=indicators.html
 - jupyter nbconvert notebooks/btc_vs_xau.ipynb --to html --no-input --output-dir=data-vision-site/docs/notebooks --output=btc_vs_xau.html
 

## 🔹 HTML-Seiten (mit Input-Zellen) generieren

 
 - jupyter nbconvert --to html notebooks/btc.ipynb
 - jupyter nbconvert --to html notebooks/indicators.ipynb
 - jupyter nbconvert --to html notebooks/xau.ipynb
 - jupyter nbconvert --to html notebooks/btc_vs_xau.ipynb
 

## 🔹 PDFs generieren

 - jupyter nbconvert notebooks/btc.ipynb --to pdf --output ../data-vision-site/docs/notebooks/files/btc.pdf
 - jupyter nbconvert notebooks/xau.ipynb --to pdf --output ../data-vision-site/docs/notebooks/files/xau.pdf
 - jupyter nbconvert notebooks/btc_vs_xau.ipynb --to pdf --output ../data-vision-site/docs/notebooks/files/btc_vs_xau.pdf
 - jupyter nbconvert notebooks/indicators.ipynb --to pdf --output ../data-vision-site/docs/notebooks/files/indicators.pdf

---

> **Tools zur Umwandlung von Notebooks in PDFs:**  
> - [miktex.org](https://miktex.org/download)  
> - [pandoc 3.7.0.2](https://github.com/jgm/pandoc/releases/tag/3.7.0.2)