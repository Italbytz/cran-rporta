# rPorta — R Interface to PORTA

> **Paket:** `rPorta` (Version 0.1-9)  
> **Autoren:** Robin Nunkesser, Silke Straatmann, Simone Wenzel  
> **Kontext:** SFB 475 („Komplexitätsreduktion in multivariaten Datenstrukturen“), TU Dortmund  
> **Lizenz:** GNU General Public License (GPL >= 2)  
> **Zugehörige Publikation:** `articles/2008/rporta/` (useR! 2008)

---

## Übersicht

`rPorta` bietet eine R-Schnittstelle zur modifizierten Version von **PORTA** (*Polyhedron Representation Transformation Algorithm*, Zuse Institute Berlin / Christof & Löbel).

### Kernfunktionalität
- **Double Description Pair:** Transformation zwischen der Scheitelpunkt-/Spannform (Konvexe Kegel / Polytope als Vektormenge) und der Facettenform (System linearer Gleichungen und Ungleichungen).
- **Zugehörigkeitsprüfungen:** Schnelle Prüfung, ob gegebene Punkte innerhalb oder außerhalb eines Polyeders liegen.
- **Fehlertoleranz-Regionen & Parameterraum-Restriktionen:** Analyse robuster Parameterschranken in multivariaten Daten.

### Struktur
- `R/`: S4-Klassen (`ieq`, `poi`, `paramspacerestriction`), Transformationsmethoden (`traf`, `fmel`, `fctp`, `vint`).
- `src/`: C-Quellcode von PORTA, Schnittstellenroutinen und exakte Arithmetik.
- `man/`: R-Dokumentation aller Klassen und Methoden.
