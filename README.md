# Max Akustik - Website Dokumentation

## 📋 Übersicht
Eine minimalistische, professionelle Website für Veranstaltungstechnik mit schwarzem Hintergrund und Lichtkegel-Effekten.

## 🎨 Design-Konzept
- **Farbschema**: Tiefschwarz (#0a0a0a) mit helweißer Schrift (#f5f5f5)
- **Akzentfarben**: Gold (#ffd700) und Blau (#4a9eff)
- **Stil**: Minimalistisch, aber aussagekräftig
- **Besonderheit**: Animierte Lichtkegel-Effekte im Hero-Bereich

## 📁 Dateien
1. **max-akustik-website.html** - Hauptwebsite (Single-Page)
2. **impressum.html** - Separate Impressum-Seite

## ⚙️ Anpassungen vornehmen

### 1. Farben ändern
Im `<style>`-Bereich finden Sie die CSS-Variablen:
```css
:root {
    --schwarz: #0a0a0a;        /* Hintergrundfarbe */
    --weiss: #f5f5f5;          /* Textfarbe */
    --akzent-gelb: #ffd700;    /* Hauptakzent */
    --akzent-blau: #4a9eff;    /* Sekundärakzent */
    --grau: #888;              /* Dezente Texte */
}
```

### 2. Kontaktdaten aktualisieren

**In der Hauptdatei (max-akustik-website.html):**
- Suchen Sie nach `<!-- HIER Ihre Telefonnummer einfügen -->`
- Suchen Sie nach `<!-- HIER Ihre E-Mail einfügen -->`
- Suchen Sie nach `<!-- HIER Ihren Standort einfügen -->`

**Im Impressum (impressum.html):**
- Ersetzen Sie alle Platzhalter-Daten unter den Überschriften

### 3. Texte personalisieren

**Über mich Sektion:**
```html
<div class="about-text">
    <p>
        <!-- HIER können Sie Ihren persönlichen Text einfügen -->
    </p>
</div>
```

**Hero-Bereich:**
Passen Sie die Hauptbotschaft direkt im HTML an.

### 4. Leistungen hinzufügen/entfernen

Suchen Sie nach:
```html
<div class="leistung-card">
    <h3>Titel der Leistung</h3>
    <p>Beschreibung</p>
    <ul>
        <li>Punkt 1</li>
        <li>Punkt 2</li>
    </ul>
</div>
```

### 5. Equipment-Liste anpassen

Suchen Sie nach:
```html
<div class="equipment-kategorie">
    <h3>Kategorie</h3>
    <ul>
        <li>Equipment 1</li>
        <li>Equipment 2</li>
    </ul>
</div>
```

### 6. Bilder einfügen

**Für die Fotogalerie:**
Ersetzen Sie die Platzhalter-Divs:
```html
<!-- Vorher: -->
<div class="galerie-item">
    <div class="galerie-overlay">...</div>
</div>

<!-- Nachher: -->
<div class="galerie-item">
    <img src="bilder/projekt1.jpg" alt="Projekt Beschreibung" style="width:100%; height:100%; object-fit:cover;">
    <div class="galerie-overlay">...</div>
</div>
```

**Für das Über-Mich Foto:**
```html
<div class="about-image">
    <img src="bilder/max-portrait.jpg" alt="Max Akustik" style="width:100%; height:100%; object-fit:cover; border-radius:10px;">
</div>
```

### 7. Formular-Funktion einrichten

Das Kontaktformular verwendet aktuell eine Platzhalter-Funktion:
```javascript
function handleFormSubmit(event) {
    // HIER Ihre eigene Logik einfügen
}
```

**Optionen:**
- **E-Mail-Service**: Formspree, EmailJS, oder SendGrid
- **PHP-Backend**: Eigenes Skript auf dem Server
- **Beispiel mit Formspree:**
```html
<form action="https://formspree.io/f/IHR_FORMSPREE_ID" method="POST">
```

## 📱 Responsive Design
Die Website ist vollständig responsive und passt sich automatisch an:
- Desktop (>768px)
- Tablet (768px - 480px)
- Mobile (<480px)

## 🚀 Installation

1. Laden Sie beide HTML-Dateien in Ihr Webhosting hoch
2. Erstellen Sie einen `bilder/` Ordner für Ihre Fotos
3. Passen Sie alle mit `<!-- HIER ... -->` markierten Stellen an
4. Testen Sie die Website lokal im Browser
5. Veröffentlichen Sie die Website

## 🔧 Erweiterte Anpassungen

### Navigation erweitern
Fügen Sie neue Links in der Navigation hinzu:
```html
<nav>
    <ul>
        <li><a href="#neue-sektion">Neuer Link</a></li>
    </ul>
</nav>
```

### Neue Sektion hinzufügen
```html
<section id="neue-sektion">
    <h2>Überschrift</h2>
    <div>Ihr Inhalt</div>
</section>
```

### Schriftgrößen anpassen
```css
:root {
    --text-klein: 0.9rem;
    --text-normal: 1.1rem;
    --text-gross: 1.8rem;
    --text-hero: 3.5rem;
}
```

## ⚡ Performance-Tipps
1. Bilder optimieren (max. 200KB pro Bild)
2. WebP-Format für bessere Kompression verwenden
3. Lazy-Loading für Bilder aktivieren:
   ```html
   <img loading="lazy" src="bild.jpg" alt="...">
   ```

## 🎯 SEO-Optimierung
1. Title-Tag anpassen
2. Meta-Beschreibung hinzufügen:
   ```html
   <meta name="description" content="Ihre Beschreibung">
   ```
3. Alt-Texte für alle Bilder hinzufügen

## 📞 Support & Fragen
Bei Fragen zur Anpassung können Sie die Kommentare im Code als Leitfaden nutzen.
Alle wichtigen Stellen sind mit `<!-- HIER ... -->` markiert.

## ✅ Checkliste vor Veröffentlichung
- [ ] Alle Kontaktdaten aktualisiert
- [ ] Impressum ausgefüllt
- [ ] Eigene Texte eingefügt
- [ ] Bilder hochgeladen und eingebunden
- [ ] Formular-Funktion getestet
- [ ] Auf verschiedenen Geräten getestet
- [ ] Rechtschreibung geprüft
- [ ] Links funktionieren

Viel Erfolg mit Ihrer neuen Website! 🎵✨
