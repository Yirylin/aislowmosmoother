# HTML Cheat Sheet — Kicoop Reference

Kompakte Übersicht der wichtigsten HTML-Tags  
für deine Webseiten und UI-Elemente (Stand 2025).

---

## Grundstruktur einer HTML-Seite

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meine Webseite</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Willkommen!</h1>
  <p>Dies ist ein Absatz mit <b>fett</b> und <i>kursiv</i>.</p>
</body>
</html>

## Text & Absätze
**Funktion Tag	Beispiel**
- Neuer Absatz	<p>	<p>Ein neuer Absatz</p>
- Zeilenumbruch	<br>	Erste Zeile<br>Zweite Zeile
- Fett	<b> oder <strong>	<strong>Wichtig!</strong>
- Kursiv	<i> oder <em>	<em>Betonung</em>
- Unterstrichen	<u>	<u>Unterstrichen</u>
- Linie/Trenner	<hr>	---

## Überschriften
**Ebene	Tag	Beispiel**
Haupttitel	<h1>	<h1>AI SlowmoSmoother</h1>
Untertitel	<h2>	<h2>Features</h2>
Unterpunkt	<h3>	<h3>Export-Modi</h3>

## Listen
**Typ	Struktur	Beispiel**
Punktliste	<ul><li>Item</li></ul>	<ul><li>Eintrag</li><li>Zweiter</li></ul>
Nummeriert	<ol><li>Item</li></ol>	<ol><li>Erster</li><li>Zweiter</li></ol>
Definitionsliste	<dl><dt>Begriff</dt><dd>Bedeutung</dd></dl>	Glossar-Stil

## Links & Bilder
**Funktion	Tag	Beispiel**
Link	<a href="ziel.html">Text</a>	<a href="privacy-policy.html">Privacy Policy</a>
Neues Fenster	<a href="url" target="_blank">	Öffnet extern
Bild	<img src="assets/logo.png" alt="Logo">	Zeigt Bild an

## Struktur & Layout
**Funktion	Tag	Beispiel**
Abschnitt	<section>	Inhaltlich verbundene Gruppe
Kopfbereich	<header>	Titel, Navigation
Fußbereich	<footer>	Impressum, Links
Container	<div>	Für Layout & Gruppierung
Zentrierung	<div style="text-align:center;">...</div>	Zentriert Text oder Bild

## Spezial
**Zweck	Tag	Beschreibung**
Code inline	<code>	Monospace-Text für Befehle
Kommentar	<!-- ... -->	Wird nicht im Browser angezeigt
Symbol	&copy;, &nbsp;, &#9733;	©, Leerzeichen, Sterne usw.

## Tipps
- HTML ist nicht case-sensitive (aber konventionell klein geschrieben).
- <br>, <hr>, <img> sind self-closing Tags — sie brauchen kein </br>.
- Nutze Einrückungen (2–4 Leerzeichen) für bessere Lesbarkeit.
- Füge <meta name="description"> & <meta name="keywords"> hinzu für SEO.
- Immer alt="" bei Bildern: wichtig für Barrierefreiheit & Google.

## Empfohlenes Zusatzwissen:
CSS Cheat Sheet (bald in docs/CSS_Cheat_Sheet.md)
HTML Validator: https://validator.w3.org/
Farbtools: https://coolors.co/

## Punktliste
.privacy ul {
  margin-left: 1.2rem;
}

/* Fix indentation for lists in Privacy section */
.privacy ul {
  list-style-position: inside;   /* Punkte bleiben innerhalb der Box */
  padding-left: 0;               /* Kein zusätzlicher linker Rand */
  margin-left: 0;                /* bündig mit Überschriften */
}

.privacy ul {
  list-style-position: outside;  /* Punkte außerhalb */
  padding-left: 1.2rem;          /* minimaler linker Abstand */
  margin-left: 0;
}

© 2025 Kicoop Interactive — Created with Resonance ✨
