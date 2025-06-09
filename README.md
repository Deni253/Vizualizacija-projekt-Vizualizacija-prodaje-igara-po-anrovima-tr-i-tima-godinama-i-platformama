# 🎮 Global Video Game Sales Dashboard

Ovaj interaktivni dashboard izrađen je pomoću **D3.js v7** i prikazuje prodaju videoigara po žanrovima, tržištima i platformama. Vizualizacija koristi **bar chart**, **pie chart**, **line chart** i **slider** za odabir godine. Projekt koristi stvarne podatke o prodaji (CSV) i omogućuje korisniku da istražuje tržišne trendove i najprodavanije igre u vremenskom rasponu.

---

## 🔧 Tehnologije korištene

- [D3.js v7](https://d3js.org/)
- [Bootstrap 5](https://getbootstrap.com/)
- HTML5 + CSS3 + JavaScript (ES6)
- [CSV dataset: `vgsales.csv`](https://www.kaggle.com/datasets/gregorut/videogame-sales-with-ratings)

---

## 📊 Funkcionalnosti

- **Slider** za odabir godine
- **Bar chart**: prodaja igara po žanrovima
- **Pie chart**: tržišni udio (EU, NA, JP, Other)
  - Klikom na segment prikaz filtrira prodaju po odabranom tržištu
  - Gumb za reset tržišta
- **Line chart**: prodaja po platformama i žanrovima
  - Klik na legendu za uključivanje/isključivanje platformi
  - Hover nad točkama prikazuje tooltip s detaljima
- **Tooltip** s informacijama o top igri i prodaji
- **Animacije** pri promjeni godine i klikovima

---

## 🗂️ Struktura projekta

/
├── index.html # Glavni HTML dokument s D3.js vizualizacijom
├── stylesheet.css # Stilovi za grafove i layout
├── vgsales.csv # Dataset s informacijama o videoigrama
└── README.md # Dokumentacija projekta
---

## ▶️ Kako pokrenuti projekt

1. Preuzmi ili kloniraj repozitorij.
2. Otvori `index.html` koristeći **Live Server** (npr. Visual Studio Code ekstenzija).
3. Provjeri da je `vgsales.csv` u istom direktoriju.
4. Interaktivni dashboard odmah će se učitati i biti spreman za korištenje.

📌 **Napomena**: Ne možeš otvoriti datoteku direktno dvoklikom jer CSV ne može biti učitan zbog CORS ograničenja u lokalnom pregledniku – koristi **Live Server**.

---

## 📚 Korištene D3 metode (izabrano)

- `d3.csv()` – učitavanje podataka iz CSV
- `d3.group()`, `d3.rollup()` – grupiranje i agregiranje
- `d3.pie()`, `d3.arc()` – kružni graf
- `d3.line()` – linijski graf
- `d3.scaleLinear()`, `d3.scaleBand()` – skale
- `d3.transition()`, `attrTween()`, `d3.interpolate()` – animacije
- `d3.drag()` – funkcionalnost kliznika
- `d3.pointer()` – pozicija pokazivača za tooltip
