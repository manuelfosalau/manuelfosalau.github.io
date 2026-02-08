# Ghid: Cum să adaugi imagini de fundal la butoane / Guide: How to Add Background Images to Buttons

## 📸 Pasul 1: Pregătește imaginile / Prepare Your Images

**Creează un folder "images" lângă fișierele HTML:**
```
your-website/
├── index.html
├── styles.css
├── images/              ← CREEAZĂ ACEST FOLDER / CREATE THIS FOLDER
│   ├── cercetare.jpg
│   ├── informatica.jpg
│   ├── gis.jpg
│   ├── metodologie.jpg
│   └── resurse.jpg
```

**Recomandări pentru imagini / Image Recommendations:**
- Format: JPG sau PNG
- Dimensiune: 800x600 pixeli (sau similar)
- Mărime fișier: Sub 500KB (pentru viteză)
- Subiect: Imagini legate de fiecare curs

---

## 🎨 Pasul 2: Înlocuiește imaginile în styles.css / Replace Images in styles.css

**Găsește această secțiune în styles.css (linia ~160):**

```css
/* === INDIVIDUAL BUTTON BACKGROUNDS === */
/* Replace the image URLs below with your own images */

/* Button 1: Cercetare și publicații */
.nav-button:nth-child(1) {
    background-image: url('images/cercetare.jpg');
}

/* Button 2: Informatică aplicată în turism */
.nav-button:nth-child(2) {
    background-image: url('images/informatica.jpg');
}

/* Button 3: GIS Applied in Tourism */
.nav-button:nth-child(3) {
    background-image: url('images/gis.jpg');
}

/* Button 4: Metodologia evaluării resurselor turistice */
.nav-button:nth-child(4) {
    background-image: url('images/metodologie.jpg');
}

/* Button 5: Resurse de învățare */
.nav-button:nth-child(5) {
    background-image: url('images/resurse.jpg');
}
```

**Înlocuiește numele fișierelor cu ale tale!**

---

## 💡 Exemple de imagini pe care le-ai putea folosi / Example Images You Could Use

**Pentru "Cercetare și publicații":**
- Cărți pe bibliotecă
- Hartă urbană
- Vedere aeriană oraș
- Conferință academică

**Pentru "Informatică aplicată în turism":**
- Computer cu date turistice
- Website de rezervări
- Dashboard analitice
- Tehnologie și turism

**Pentru "GIS Applied in Tourism":**
- Hartă GIS colorată
- QGIS screenshot
- Analiză spațială
- Hartă turistică

**Pentru "Metodologie":**
- Grafice și diagrame
- Chestionare
- Analiza datelor
- Resurse turistice evaluate

**Pentru "Resurse de învățare":**
- Cărți și laptop
- Bibliotecă
- Student învățând
- Materiale educaționale

---

## 🔍 Unde să găsești imagini gratuite / Where to Find Free Images

**Site-uri cu imagini gratuite (fără drepturi de autor):**
- https://unsplash.com/
- https://pexels.com/
- https://pixabay.com/

**Caută termeni ca:**
- "urban planning"
- "GIS map"
- "tourism research"
- "geography study"
- "data analysis"

---

## ⚙️ Ajustarea transparenței / Adjusting Transparency

**Transparența este acum 50% (0.5). Dacă vrei să o schimbi:**

**În styles.css, găsește:**
```css
.nav-button::after {
    background: rgba(255, 255, 255, 0.5); /* 50% transparent */
}
```

**Schimbă valoarea:**
- `0.3` = Mai transparentă (imaginea se vede mai mult)
- `0.5` = Mediu (implicit)
- `0.7` = Mai opacă (textul se vede mai bine)

---

## 🎨 Opțiuni alternative pentru text / Alternative Text Options

**Dacă vrei text într-un dreptunghi colorat în loc de alb semi-transparent:**

În styles.css, schimbă:
```css
.nav-button h3 {
    background: rgba(103, 126, 234, 0.9); /* Albastru semi-transparent */
    color: white; /* Text alb */
    padding: 0.5rem 1rem;
    border-radius: 8px;
}
```

**Sau pentru un oval:**
```css
.nav-button h3 {
    background: rgba(255, 255, 255, 0.9);
    padding: 0.5rem 1.5rem;
    border-radius: 30px; /* Face oval */
}
```

---

## 🚨 Dacă imaginile nu apar / If Images Don't Show

**Verifică:**
1. ✓ Folderul "images" este lângă index.html?
2. ✓ Numele fișierelor sunt corecte? (case-sensitive!)
3. ✓ Extensia este corectă? (.jpg nu .JPG)
4. ✓ Calea în CSS este corectă?

**Testează cu o imagine simplă:**
```css
.nav-button:nth-child(1) {
    background-image: url('images/test.jpg');
    background-color: red; /* Dacă vezi roșu, imaginea lipsește */
}
```

---

## 📝 Rezumat rapid / Quick Summary

1. **Creează folder "images"** lângă index.html
2. **Pune 5 imagini** în folder (cercetare.jpg, informatica.jpg, etc.)
3. **Asigură-te că numele din styles.css** corespund cu numele imaginilor tale
4. **Deschide index.html** în browser și verifică!

---

**Întrebări? Întreabă-mă!** / **Questions? Ask me!**
