# HTML-Grundlagen

HTML ist die Sprache, die das Grundgerüst einer Webseite bildet. Mit HTML sagst du dem Browser, welche Art von Inhalten abgebildet sind. Hier sind die wichtigsten **HTML-Tags** (Elemente), die dir am Anfang helfen, deine eigene Webseite zu erstellen:

---

## Überschriften: `h1`, `h2`, `h3`

Mit Überschriften kannst du Texte unterschiedlich wichtig machen. Die Zahlen `1` bis `6` zeigen, wie wichtig eine Überschrift ist, wobei `h1` die wichtigste ist.

```html
<h1>Das ist eine große Überschrift</h1>
<h2>Das ist eine mittlere Überschrift</h2>
<h3>Das ist eine kleine Überschrift</h3>
```

---

## Absätze: `p`

Ein Absatz (`p`) wird genutzt, um einen normalen Text zu schreiben. So kannst du deinen Inhalt gut lesbar machen.

```html
<p>Dies ist ein normaler Absatz. Hier steht dein Text.</p>
```

---

## Links: `a`

Mit dem `a`-Tag erstellst du einen Link, mit dem die Nutzer auf eine andere Webseite springen können. Der Text zwischen den Tags ist klickbar.

```html
<a href="https://www.example.com">Klick mich!</a>
```

---

## Buttons: `button`

Ein `button` ist ein Knopf, den man anklicken kann, um Aktionen auszulösen.

```html
<button>Drück mich!</button>
```

---

## Listen: `ul`, `li`

Mit `ul` kannst du eine ungeordnete Liste (Bullet-Points) erstellen. Jedes Listenelement steht in einem `li`.

```html
<ul>
  <li>Erstes Listenelement</li>
  <li>Zweites Listenelement</li>
</ul>
```

Es gibt auch **nummerierte Listen** mit `ol` (ordered list):

```html
<ol>
  <li>Erstes Element</li>
  <li>Zweites Element</li>
</ol>
```

---

## Container: `div` und `span`

`div` und `span` sind wichtige Tags, um Inhalte zu gruppieren oder zu organisieren.

- **`div`** ist ein Blockelement, das meist für größere Abschnitte verwendet wird.
- **`span`** ist ein Inline-Element, das für kleinere Textteile oder Elemente benutzt wird.

```html
<div>
  <h2>Ein Bereich</h2>
  <p>Hier steht ein Text innerhalb des div-Bereichs.</p>
</div>

<p>Ein normaler Text mit einem <span>hervorgehobenen Teil</span>.</p>
```

---

## Bilder: `img`

Mit dem `img`-Tag kannst du ein Bild auf deiner Webseite anzeigen. Du musst die Quelle des Bildes mit dem `src`-Attribut angeben.

```html
<img src="https://example.com/bild.jpg" alt="Beschreibung des Bildes">
```

---

## Zusammenfassung

Diese HTML-Tags helfen dir, die Grundstruktur deiner Webseite zu erstellen. Du kannst sie kombinieren, um Texte, Links, Listen und Buttons zu bauen. Probiere einfach aus, sie auf einer Webseite zu verwenden und beobachte, wie sich die Seite verändert!