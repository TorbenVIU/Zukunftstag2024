# JavaScript-Grundlagen

JavaScript ist die Programmiersprache, die deiner Webseite **Interaktivität** verleiht. Mit JavaScript kannst du auf Klicks reagieren, Inhalte verändern oder Daten speichern. Hier sind die wichtigsten JavaScript-Konzepte für den Einstieg:

---

## 1. HTML-Elemente auswählen: `querySelector`

Mit `querySelector` kannst du HTML-Elemente mit CSS-Selektoren auswählen, um später mit ihnen zu arbeiten.

```javascript
// Wähle das erste Element mit der Klasse "highlight" aus
const element = document.querySelector(".highlight");

// Wähle ein Element mit der ID "button"
const button = document.querySelector("#button");
```

---

## 2. Auf Klicks reagieren: `addEventListener`

Mit `addEventListener` kannst du auf Benutzeraktionen reagieren, z.B. auf einen **Klick**. Das ist besonders nützlich, um Buttons interaktiv zu machen.

### Beispiel: Ein Button, der eine Nachricht in der Konsole anzeigt

Im HTML:

```html
<button id="clickButton">Klick mich!</button>
```

Im JavaScript:

```javascript
const button = document.querySelector("#clickButton");

button.addEventListener("click", function () {
  console.log("Der Button wurde geklickt!");
});
```

---

## 3. Klassen hinzufügen oder entfernen: `classList.toggle`

Mit `classList.toggle` kannst du einer HTML-Komponente Klassen hinzufügen oder entfernen. Das ist praktisch, um ein Element sichtbar oder unsichtbar zu machen oder das Design zu ändern.

### Beispiel: Ein Button, der eine Klasse hinzufügt/entfernt

Im HTML:

```html
<div id="box" class="hidden">Ich werde versteckt!</div>
<button id="toggleButton">Anzeigen/Verstecken</button>
```

Im CSS:

```css
.hidden {
  display: none;
}
```

Im JavaScript:

```javascript
const box = document.querySelector("#box");
const toggleButton = document.querySelector("#toggleButton");

toggleButton.addEventListener("click", function () {
  box.classList.toggle("hidden");
});
```

Wenn du den Button klickst, wird das `div`-Element angezeigt oder versteckt, je nachdem, ob die Klasse `hidden` aktiv ist oder nicht.

---

## 4. Den Inhalt eines Elements ändern: `innerText` und `innerHTML`

Mit `innerText` oder `innerHTML` kannst du den Text oder den HTML-Inhalt eines Elements ändern.

### Beispiel: Den Text eines Absatzes ändern

Im HTML:

```html
<p id="text">Hier steht alter Text.</p>
<button id="changeTextButton">Ändere den Text!</button>
```

Im JavaScript:

```javascript
const textElement = document.querySelector("#text");
const changeTextButton = document.querySelector("#changeTextButton");

changeTextButton.addEventListener("click", function () {
  textElement.innerText = "Hier steht neuer Text!";
});
```

---

## 5. Variablen und Funktionen

### Variablen

In JavaScript speicherst du Daten in **Variablen**. Es gibt zwei Schlüsselwörter, um Variablen zu erstellen: `let` und `const`.

```javascript
let name = "Anna"; // Eine veränderbare Variable
const pi = 3.14159; // Eine unveränderbare Konstante
```

### Funktionen

Eine Funktion ist eine Gruppe von Befehlen, die du mehrfach aufrufen kannst.

```javascript
function sagHallo() {
  console.log("Hallo!");
}

sagHallo(); // Ruft die Funktion auf und zeigt 'Hallo!' in der Konsole an
```

---

## 6. Schleifen: `for`

Mit Schleifen kannst du Code wiederholt ausführen. Die `for`-Schleife ist besonders nützlich, um Listen oder Arrays zu durchlaufen.

### Beispiel: Durch eine Liste von Zahlen zählen

```javascript
for (let i = 1; i <= 5; i++) {
  console.log(i); // Gibt 1 bis 5 in der Konsole aus
}
```

---

## 7. Arrays: Listen von Werten

Ein **Array** ist eine Liste von Werten, die du in einer einzigen Variable speichern kannst. Arrays sind nützlich, wenn du mehrere Daten auf einmal speichern möchtest, wie zum Beispiel Namen oder Zahlen.

### Beispiel: Ein Array erstellen

```javascript
let zahlen = [1, 2, 3, 4, 5];
let namen = ["Anna", "Ben", "Clara"];
```

### Elemente aus einem Array abrufen

Du kannst auf einzelne Werte eines Arrays zugreifen, indem du den **Index** verwendest (die Position des Elements, beginnend bei 0).

```javascript
console.log(namen[0]); // Gibt "Anna" aus
console.log(zahlen[2]); // Gibt "3" aus
```

### Durch ein Array iterieren

Mit einer **Schleife** kannst du durch alle Elemente eines Arrays gehen:

```javascript
let zahlen = [1, 2, 3, 4, 5];

for (let i = 0; i < zahlen.length; i++) {
  console.log(zahlen[i]); // Gibt 1, 2, 3, 4, 5 aus
}
```

### Arrays manipulieren

- **`push()`**: Fügt ein neues Element am Ende des Arrays hinzu.
- **`pop()`**: Entfernt das letzte Element aus dem Array.

```javascript
let zahlen = [1, 2, 3];
zahlen.push(4); // Zahlen ist jetzt [1, 2, 3, 4]
zahlen.pop(); // Zahlen ist jetzt [1, 2, 3]
```

---

Arrays sind eine mächtige Möglichkeit, um viele Daten zu speichern und zu bearbeiten. Du wirst sie in fast jedem JavaScript-Projekt verwenden!

## Zusammenfassung

JavaScript bringt Bewegung in deine Webseite! Mit `querySelector` wählst du HTML-Elemente aus, und mit `addEventListener` machst du sie interaktiv. Funktionen wie `classList.toggle`, `innerText` und `innerHTML` helfen dir dabei, Inhalte zu verändern oder Klassen hinzuzufügen. Variablen und Schleifen machen es einfach, deine Programme dynamischer und flexibler zu gestalten.
