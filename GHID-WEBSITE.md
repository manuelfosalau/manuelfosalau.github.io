# Ghid pentru site-ul tău academic / Guide for Your Academic Website

## 📁 Ce ai primit / What You Got

### Fișiere HTML (9 pagini / 9 pages):
1. **index.html** - Pagina principală cu butoane mari / Main page with large buttons
2. **acasa.html** - Despre tine / About you
3. **cercetare.html** - Cercetare și publicații / Research and publications
4. **informatica-turism.html** - Curs: Informatică aplicată în turism
5. **gis-tourism.html** - Course: GIS Applied in Tourism (English)
6. **metodologie.html** - Curs: Metodologia evaluării resurselor turistice
7. **resurse.html** - Resurse de învățare / Learning resources

### Fișiere CSS (2):
8. **styles.css** - Stiluri pentru pagina principală / Styles for main page
9. **styles-pages.css** - Stiluri pentru celelalte pagini / Styles for other pages

---

## 🎯 Structura site-ului / Website Structure

```
Pagina principală (index.html)
│
├─ Titlu MARE (decizi tu) / LARGE Title (you decide)
├─ Subtitlu / Subtitle
│
└─ 6 Butoane mari stilizate / 6 Large stylized buttons:
    ├─ Acasă
    ├─ Cercetare și publicații
    ├─ Informatică aplicată în turism
    ├─ GIS Applied in Tourism
    ├─ Metodologia evaluării resurselor turistice
    └─ Resurse de învățare
│
└─ Contact (jos de tot) / Contact (at bottom)
    ├─ Email
    └─ LinkedIn
```

---

## ✏️ Cum să personalizezi / How to Customize

### PASUL 1: Schimbă titlul mare / Change the large title

**În index.html, găsește:**
```html
<h1 class="main-title">YOUR TITLE HERE</h1>
<p class="subtitle">Add your subtitle or tagline here</p>
```

**Înlocuiește cu (exemple):**
```html
<h1 class="main-title">Dr. Numele Tău</h1>
<p class="subtitle">Geografie • Turism • GIS</p>
```

SAU / OR:

```html
<h1 class="main-title">Geografia Turismului</h1>
<p class="subtitle">Materiale didactice și cercetare</p>
```

---

### PASUL 2: Adaugă datele tale de contact / Add your contact data

**În index.html, jos de tot, găsește:**
```html
<p>
    <strong>Email:</strong> 
    <a href="mailto:your.email@university.edu">your.email@university.edu</a>
</p>
<p>
    <strong>LinkedIn:</strong> 
    <a href="https://www.linkedin.com/in/your-profile" target="_blank">
        linkedin.com/in/your-profile
    </a>
</p>
```

**Înlocuiește cu datele tale reale:**
```html
<p>
    <strong>Email:</strong> 
    <a href="mailto:manu.example@uaic.ro">manu.example@uaic.ro</a>
</p>
<p>
    <strong>LinkedIn:</strong> 
    <a href="https://www.linkedin.com/in/manu-geografia" target="_blank">
        linkedin.com/in/manu-geografia
    </a>
</p>
```

---

### PASUL 3: Personalizează paginile cu conținut / Customize content pages

#### A) Pagina "Acasă" (acasa.html)

Schimbă:
- Despre tine
- Domeniile de cercetare
- Educația ta
- Experiența didactică

#### B) Pagina "Cercetare" (cercetare.html)

Adaugă publicațiile tale:
```html
<div class="publication-item">
    <h3>Titlul lucrării tale</h3>
    <p class="publication-meta">Revista, 2024</p>
    <p class="publication-description">
        Descrierea lucrării...
    </p>
    <a href="https://drive.google.com/file/d/..." target="_blank">Descarcă PDF</a>
</div>
```

#### C) Paginile de curs

**Pentru fiecare curs (informatica-turism.html, gis-tourism.html, metodologie.html):**

1. **Adaugă link-uri către materialele tale de pe Google Drive:**

```html
<li>
    <a href="https://drive.google.com/file/d/ABC123XYZ/view" target="_blank">
        Cursul 1 - Titlul cursului
    </a>
</li>
```

2. **Cum să obții link-ul Google Drive:**
   - Intră în Google Drive
   - Click dreapta pe fișier → "Partajează" / "Share"
   - "Oricine cu linkul" / "Anyone with the link" → "Vizualizator" / "Viewer"
   - Copiază linkul
   - Lipește-l în HTML

3. **Pentru un folder întreg:**
```html
<li>
    <a href="https://drive.google.com/drive/folders/FOLDER-ID" target="_blank">
        📁 Toate materialele de curs
    </a>
</li>
```

---

## 🎨 Cum să schimbi culorile / How to Change Colors

### În styles.css (pentru pagina principală):

**Fundal gradient mare / Large gradient background:**
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```
Schimbă codurile hex cu culorile tale preferate!

**Culoarea butoanelor / Button colors:**
```css
border-top: 4px solid #667eea;  /* Linia de sus / Top line */
border-color: #667eea;  /* Bordura la hover / Border on hover */
```

**Instrumente utile pentru culori / Useful color tools:**
- https://coolors.co/ - Generator de palete
- https://htmlcolorcodes.com/ - Selector de culori

---

## 🔗 Despre link-uri / About Links

### Tipuri de link-uri / Types of links:

**1. Link către altă pagină a site-ului tău:**
```html
<a href="cercetare.html">Cercetare</a>
```

**2. Link către fișier PDF pe Google Drive:**
```html
<a href="https://drive.google.com/file/d/YOUR-FILE-ID/view" target="_blank">
    Cursul 1 (PDF)
</a>
```

**3. Link către un site extern:**
```html
<a href="https://www.qgis.org/" target="_blank">
    QGIS Software
</a>
```

**4. Link către email:**
```html
<a href="mailto:your@email.com">Email-ul tău</a>
```

**Nota:** `target="_blank"` face ca link-ul să se deschidă într-un tab nou!

---

## 📱 Testare / Testing

### Înainte de a pune online / Before publishing:

1. **Descarcă toate fișierele**
2. **Pune-le într-un folder**
3. **Dublu-click pe index.html**
4. **Testează:**
   - Toate butoanele funcționează?
   - Toate link-urile merg unde trebuie?
   - Arată bine pe telefon? (redimensionează fereastra browserului)

---

## 🌐 Cum să publici online / How to Publish Online

### Opțiunea 1: GitHub Pages (GRATUIT / FREE)

1. Creează cont pe github.com
2. Creează repository nou: `username.github.io`
3. Încarcă toate fișierele HTML și CSS
4. Site-ul va fi live la: `https://username.github.io`

**Avantaje:**
- ✓ Gratuit / Free
- ✓ Popular în mediul academic
- ✓ Ușor de actualizat / Easy to update

### Opțiunea 2: Netlify (FOARTE UȘOR / VERY EASY)

1. Mergi pe netlify.com
2. Trage folderul cu fișiere (drag & drop)
3. Primești URL instant / Get instant URL

### Opțiunea 3: Server universitate / University server

Multe universități oferă hosting gratuit pentru cadre didactice!
Contactează departamentul IT.

---

## 🎓 Sfaturi / Tips

### Pentru organizarea materialelor pe Google Drive:

```
📁 Materiale Didactice/
├── 📁 Informatică Turism/
│   ├── 📁 Cursuri/
│   │   ├── Curs1.pdf
│   │   └── Curs2.pdf
│   └── 📁 Teme/
│       └── Tema1.pdf
├── 📁 GIS Tourism/
│   ├── 📁 Lectures/
│   └── 📁 Lab Materials/
└── 📁 Metodologie/
    └── ...
```

**Apoi partajează fiecare folder și adaugă link-ul pe site!**

---

## 🆘 Întrebări frecvente / FAQ

**Î: Trebuie să descarc fișierele acum?**
R: Nu! Poți continua să le editezi aici. Descarcă când e totul gata.

**Î: Pot schimba emoji-urile de pe butoane?**
R: Da! În index.html, schimbă emoji-urile:
```html
<div class="button-icon">🏠</div>  <!-- Orice emoji vrei -->
```

**Î: Cum adaug o poză cu mine?**
R: Întreabă-mă și îți arăt cum! E simplu.

**Î: Pot adăuga mai multe butoane?**
R: Da! Copiază structura unui buton existent și modifică.

**Î: Fonturile se vor încărca mereu?**
R: Da! Google Fonts le încarcă automat, gratuit.

**Î: Ce fac dacă "stric" ceva?**
R: Descarcă din nou fișierele originale de aici!

---

## ✨ Ce poți adăuga mai târziu / What You Can Add Later

Spune-mi dacă vrei să adăugăm:
- ✓ Poza ta pe pagina principală / Your photo on main page
- ✓ Galerie de imagini din teren / Image gallery from fieldwork
- ✓ Calendar cu orele de consultații / Office hours calendar
- ✓ Hartă interactivă / Interactive map
- ✓ Secțiune blog / Blog section
- ✓ Formular de contact / Contact form

---

## 📞 Ai nevoie de ajutor? / Need Help?

Întreabă-mă orice:
- "Cum schimb culoarea în verde?"
- "Vreau să adaug o secțiune nouă"
- "Link-ul meu Google Drive nu merge"
- "Cum pun o imagine?"

**Suntem aici să construim împreună, pas cu pas!**

---

**P.S.** Site-ul funcționează pe:
- ✓ Desktop
- ✓ Tablete
- ✓ Telefoane mobile
- ✓ Toate browserele moderne

**Totul e gata să folosești! 🎉**
