# CSS-Grundlagen

CSS (Cascading Style Sheets) ist dafür da, das Aussehen deiner Webseite zu gestalten. Während HTML das **Gerüst** liefert, sorgt CSS für das **Design**. Hier sind die wichtigsten Konzepte und Eigenschaften für den Einstieg in CSS:

---

## Selektoren: Wie du Elemente ansprichst

In CSS bestimmst du, welches Element du stylen willst. Dafür gibt es verschiedene Selektoren:

### 1. **Tag-Selektor**

Du kannst direkt HTML-Tags ansprechen, um alle Elemente eines Typs zu gestalten.

```css
p {
  color: blue;
}
```

Dieses Beispiel färbt alle `<p>`-Elemente (Absätze) auf deiner Webseite blau.

---

### 2. **Klassen-Selektor** (`.`)

Mit Klassen kannst du Elemente gezielt ansprechen. Du kannst einer Klasse mehrere Elemente zuweisen. Klassen beginnen immer mit einem Punkt (`.`).
Im CSS Dokument nutzen wir fast immer Klassen-Selektoren

Im HTML:

```html
<p class="highlight">Ich bin hervorgehoben!</p>
```

Im CSS:

```css
.highlight {
  background-color: yellow;
}
```

Dieses Beispiel gibt dem Absatz eine gelbe Hintergrundfarbe, weil er die Klasse `highlight` hat.

---

### 3. **ID-Selektor** (`#`)

Eine ID wird für ein spezifisches, einzigartiges Element genutzt. IDs beginnen mit einem Hashtag (`#`).

Im HTML:

```html
<p id="intro">Ich bin der erste Absatz!</p>
```

Im CSS:

```css
#intro {
  font-size: 20px;
}
```

Dieses Beispiel setzt die Schriftgröße für den Absatz mit der ID `intro` auf 20px.

---

## Die wichtigsten CSS-Eigenschaften

### 1. **Farbe** (`color`, `background-color`)

- `color`: Die Farbe des Textes.
- `background-color`: Die Hintergrundfarbe eines Elements.

```css
p {
  color: white;
  background-color: black;
}
```

---

### 2. **Schriftgröße** (`font-size`)

Mit `font-size` legst du fest, wie groß der Text ist.

```css
h1 {
  font-size: 36px;
}
```

---

### 3. **Abstand** (`margin`, `padding`)

- `margin`: Der äußere Abstand eines Elements (außen um das Element herum).
- `padding`: Der innere Abstand eines Elements (zwischen Inhalt und Rand).

```css
div {
  margin: 20px;
  padding: 10px;
}
```

---

### 4. **Rahmen** (`border`)

Mit `border` kannst du einen Rahmen um ein Element zeichnen.

```css
p {
  border: 2px solid black;
}
```

Dieses Beispiel erstellt einen 2 Pixel breiten, durchgehenden schwarzen Rahmen um den Absatz.

---

### 5. **Breite und Höhe** (`width`, `height`)

Du kannst die Breite und Höhe eines Elements festlegen.

```css
div {
  width: 300px;
  height: 200px;
}
```

---

### 6. **Textausrichtung** (`text-align`)

Mit `text-align` legst du fest, wie der Text innerhalb eines Elements ausgerichtet ist.

```css
h2 {
  text-align: center;
}
```

---

### 7. **Display** (`display`)

Mit `display` bestimmst du, wie ein Element dargestellt wird:

- `block`: Das Element nimmt die volle Breite ein (wie bei `div`).
- `inline`: Das Element nimmt nur so viel Platz ein, wie nötig (wie bei `span`).
- `none`: Versteckt das Element komplett.

```css
div {
  display: block;
}
span {
  display: inline;
}
```

---

## Zusammenfassung

Mit CSS kannst du deine Webseite individuell gestalten. Du hast gelernt, wie du Elemente mit Klassen, IDs oder direkt über ihren Tag ansprechen kannst. Mit den wichtigsten Eigenschaften wie Farbe, Schriftgröße, Abständen und Rahmen hast du die Werkzeuge, um loszulegen!
