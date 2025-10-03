# CSS Cheat Sheet – AI SlowmoSmoother (AISS)

Dieses Cheat-Sheet sammelt die wichtigsten CSS-Effekte für unsere Landingpage.
Jeder Abschnitt enthält Beispiele + Kommentare, damit man sie jederzeit anpassen kann.

---


## 🔹 1. Glow-Text
.glow-text {
  color: #ffd900;                        /* Textfarbe */
  text-shadow: 0 0 8px #ffd900,          /* erster Glow-Effekt */
               0 0 16px #ffd900;         /* zweiter Glow (größer, weicher) */
}
Nutze für Überschriften oder Schlagworte (<h2 class="glow-text">Features</h2>).

## 🔹 2. Glow-Box / Button
.glow-box {
  background: #0b0c10;                   /* dunkler Hintergrund */
  border: 2px solid #edfefe;             /* Rahmen */
  box-shadow: 0 0 10px #edfefe,          /* heller Glow */
              0 0 20px #ffd900;          /* zweiter, farbiger Glow */
}
Nutze für Buttons oder Container (<div class="glow-box">Text</div>).

## 🔹 3. Hover-Effekt (Aufleuchten bei Mausbewegung)
.hover-glow:hover {
  color: #ffd900;                        /* Farbe beim Hover */
  text-shadow: 0 0 8px #ffd900;          /* Glow beim Hover */
  transform: scale(1.05);                /* leichtes Vergrößern */
  transition: all 0.3s ease;             /* sanfte Animation */
}
Perfekt für Buttons oder Listenpunkte.

## 🔹 4. Pulsierende Animation
@keyframes pulse {
  0%   { transform: scale(1);   box-shadow: 0 0 8px #ffd900; }
  50%  { transform: scale(1.1); box-shadow: 0 0 20px #ffd900; }
  100% { transform: scale(1);   box-shadow: 0 0 8px #ffd900; }
}

.pulse {
  animation: pulse 2s infinite;          /* läuft endlos, 2 Sekunden pro Zyklus */
}
Nutze für leuchtende Punkte (<span class="dot pulse yellow"></span>).

## 🔹 5. Slide-In Effekt
@keyframes slideIn {
  from { opacity: 0; transform: translateY(20px); }
  to   { opacity: 1; transform: translateY(0); }
}

.slide-in {
  animation: slideIn 1s ease forwards;   /* Einmalig beim Laden */
}
Elemente erscheinen von unten hereingeschoben.

## 🔹 6. Neon-Style
.neon {
  color: #00cfff;
  text-shadow: 0 0 5px #00cfff,
               0 0 10px #00cfff,
               0 0 20px #00cfff,
               0 0 40px #00cfff;
}
Typischer Neon-Look für Logos oder Key-Words.

## 🔹 7. Responsive Anpassungen
@media (max-width: 600px) {
  h1 { font-size: 1.8rem; }              /* kleinere Schrift auf Handy */
  .btn { font-size: 0.9rem; }            /* Buttons anpassen */
}
Damit die Seite auch auf dem Smartphone gut aussieht.


