---
name: loopsystem
description: Plan-Delegieren-Prüfen-Loop. Das aktuelle Top-Modell plant und prüft, ein günstiger Haiku-Subagent setzt die einzelnen Schritte um. Auslöser: Nachricht beginnt mit «Loop:» oder der Nutzer will eine grosse, wiederholbare Aufgabe günstig erledigen lassen.
---

# Loopsystem

Teure Denkarbeit macht das grosse Modell, Fleissarbeit ein günstiges. Das spart Limit und hält die Qualität hoch.

## Auslöser

- Nachricht beginnt mit `Loop:` → immer dieses Vorgehen
- Grosse Mengenarbeit (viele Captions, viele Dateien, viele Varianten) → Loop vorschlagen

## Ablauf

### 1. Planen (Top-Modell, du selbst)
- Ziel in einem Satz festhalten.
- Aufgabe in kleine, unabhängige Arbeitspakete teilen. Jedes Paket:
  - hat einen klaren Input und ein klar beschriebenes Ergebnis
  - braucht keinen Kontext aus anderen Paketen
  - hat **Abnahmekriterien** (woran man erkennt, dass es fertig und gut ist)
- Aufgabenliste mit allen Paketen anlegen.

### 2. Delegieren (Haiku-Subagent)
- Pro Paket einen Subagent mit `model: "haiku"` starten.
- Der Auftrag ist vollständig und eigenständig: Ziel, Input, Format, Abnahmekriterien, Stilregeln (z. B. «keine Gedankenstriche, Du-Form»).
- Unabhängige Pakete parallel starten.
- Wenn keine Subagents verfügbar sind: Pakete selbst nacheinander abarbeiten und das dem Nutzer in einem Satz sagen.

### 3. Prüfen (Top-Modell)
- Jedes Ergebnis gegen seine Abnahmekriterien prüfen.
- Bestanden → abhaken.
- Nicht bestanden → konkretes Feedback formulieren und das Paket **einmal** neu delegieren. Scheitert es erneut, selbst korrigieren.

### 4. Zusammenführen
- Ergebnisse zusammensetzen, Gesamtergebnis ein letztes Mal prüfen (Konsistenz, Ton, Vollständigkeit).
- Dem Nutzer liefern: Ergebnis plus ein Satz, wie viele Pakete delegiert und wie viele nachgebessert wurden.

## Regeln

- Nie Entscheidungen delegieren, die etwas veröffentlichen, verschicken oder löschen.
- Für Pakete, die starkes Urteilsvermögen brauchen (Strategie, heikle Texte), lieber selbst arbeiten.
- Der Subagent sieht dieses Gespräch nicht: alles Nötige gehört in seinen Auftrag.
