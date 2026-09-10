# Stack & Reach — Rahmen-Fit

Ein Werkzeug, um Fahrradrahmen-Geometrien systematisch gegen die eigenen
Bikefitting-Zielwerte (Stack & Reach) zu vergleichen.

## Was es macht

- Ziel-Stack/Reach eintragen (vom Bikefitter oder selbst gemessen).
- Beliebig viele Rahmen mit Stack & Reach erfassen.
- Pro Rahmen: ΔStack, ΔReach, Stack-Reach-Verhältnis (STR) und eine
  **Kompensations-Rechnung** — lässt sich der Rahmen mit Spacern und Vorbau
  (innerhalb eines einstellbaren Budgets) auf das Ziel bringen?
- **Ampel** (passend / grenzwertig / schwierig) auf Basis der Rest-Abweichung
  *nach* der Cockpit-Korrektur, mit einstellbaren Toleranzen.
- **Zielkreuz-Diagramm** (Reach × Stack) mit den Rahmen-Endpunkten.
- Vorbau-Empfehlung in realen 10-mm-Schritten; Spacer stufenlos.

## Nutzung

Einzelne, eigenständige HTML-Datei — `index.html` im Browser öffnen.
Keine Abhängigkeiten, kein Server. Alle Daten werden lokal im Browser
gespeichert (localStorage); Export/Import als JSON ist eingebaut.

## Rechenannahmen

- Vergleichswert ist der **Rahmen**-Stack/Reach.
- Spacer heben den Stack (`h·sin(73°)`) und verkürzen den Reach (`h·cos(73°)`);
  der Steuerrohrwinkel ist fest mit 73° angesetzt (Einfluss zweiter Ordnung).
- Stack lässt sich per Spacer anheben, kaum absenken (asymmetrisches Budget).
- Reach wird über die Vorbau-Spanne ausgeglichen (10-mm-Schritte).

Ersetzt keinen Bikefitter — hilft beim systematischen Vergleich beim Rahmenkauf.
