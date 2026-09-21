# FINE — Financial Information Neural Engine

FINE ist ein KI-Experiment: Täglich (Mo–Fr) erstellt die Engine vor Börsenstart eine Prognose für 2–3 selbst gewählte, handelbare Werte (Mix DAX / US / Indizes) und reviewt diese mittags und abends gegen die tatsächliche Kursentwicklung.

**⚠️ Disclaimer:** FINE ist ein Experiment zur Bewertung von KI-Prognosen. Alle Inhalte sind **keine Anlageberatung und keine Kauf-/Verkaufsempfehlung**.

## Slots (Europe/Berlin)
| Zeit | Job | Inhalt |
|---|---|---|
| 08:30 | Morgen | Analyse, Werteauswahl, Tagesprognose (Richtung, Bandbreite, Konfidenz, Begründung) |
| 14:00 | Mittag | Zwischen-Review: Ist-Prognose vs. Kursentwicklung |
| 22:00 | Abend | Abschluss-Review, Bewertung (Treffer/Fehler), Lern-Log-Eintrag |

## Datenstruktur
- `index.html` — Dashboard (GitHub Pages)
- `data/predictions.json` — alle Prognosen & Reviews (täglich erweitert)
- `data/stats.json` — aggregierte Trefferquoten & Lernfortschritt
- `data/config.json` — Anlageuniversum & Regeln

## Lernen
FINE wertet die eigene Prognosehistorie aus und passt Auswahl-Heuristiken iterativ an (dokumentiert im Lern-Log auf der Seite).
