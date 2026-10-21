---
name: podcast-schnitt-premiere
description: Kompletter Video-Podcast-Schnitt in Adobe Premiere Pro, ferngesteuert über Computer Use: Spuren synchronisieren, Farbe angleichen, Lücken entfernen, AutoPod-Multicam, Jump Cuts, Untertitel und Intro. Nutzen, wenn eine Podcast-Folge in Premiere geschnitten werden soll.
---

# Podcast-Schnitt in Premiere Pro

Arbeitet in Premiere Pro auf dem Computer des Nutzers (über Computer Use). Zuerst den `computer-use` Skill lesen.

## 0. Vorbereitung klären (eine Rückfrage, falls unbekannt)

- Wo liegen die Rohdateien (Kameras, separate Audiospuren)?
- Wie viele Sprecher und Kameras?
- Ist das Plugin **AutoPod** installiert?
- Gibt es ein Intro, eine Bauchbinden-Vorlage, eine Farb-LUT?
- Zielformat: 16:9 YouTube, zusätzlich 9:16 Clips?

## 1. Projekt und Import
1. Neues Projekt oder bestehendes öffnen, Ordnerstruktur anlegen: `Video`, `Audio`, `Grafik`, `Sequenzen`.
2. Alle Rohdateien importieren.

## 2. Synchronisieren
1. Alle Kamera- und Audioclips markieren → Rechtsklick → **Multi-Camera-Quellsequenz erstellen**, Synchronisationspunkt **Audio**.
2. Bei Abweichungen: manuell an einer deutlichen Spitze (Klatscher) ausrichten.
3. Multicam-Sequenz in eine neue Schnittsequenz legen.

## 3. Farbe
1. Lumetri Color öffnen, pro Kamera: Weissabgleich, Belichtung, Kontrast.
2. LUT des Nutzers anwenden, falls vorhanden.
3. Kameras aneinander angleichen (Vergleichsansicht), Hauttöne prüfen.

## 4. Audio
1. Mikrofonspuren auf Dialog setzen (Essential Sound → Dialog), Lautheit automatisch anpassen.
2. Ziel: ca. −14 LUFS integriert für YouTube, Spitzen unter −1 dBTP.
3. Bei Bedarf Rauschminderung und «Sprache verbessern».

## 5. Lücken und Jump Cuts
1. Mit Text-basierter Bearbeitung (Transkript) Pausen und Füllwörter («äh», «ähm») markieren und entfernen.
2. Lange Pausen > 0,7 s kürzen, Versprecher und Wiederholungen entfernen.
3. Jump Cuts mit leichtem Zoom (105–110 %) kaschieren, wo dieselbe Kamera zweimal folgt.

## 6. AutoPod Multicam
1. AutoPod Multi-Camera Editor öffnen, Mikrofon je Sprecher der Kamera zuordnen, Weitwinkel-Anteil einstellen.
2. Schnitt erzeugen, danach stichprobenartig prüfen (Lacher, Zwischenrufe → Weitwinkel).
3. Ohne AutoPod: Multicam im Programmmonitor live umschalten oder Schnitte anhand des Transkripts setzen.

## 7. Untertitel
1. Transkript erzeugen (Sprache korrekt wählen), Fehler korrigieren, Namen prüfen.
2. Untertitel erstellen, Stil des Nutzers anwenden, max. 2 Zeilen, ca. 32 Zeichen pro Zeile.

## 8. Intro und Grafik
1. Intro an den Anfang, Übergang zum ersten Satz sauber.
2. Bauchbinden für jeden Sprecher beim ersten Auftritt.

## 9. Export
1. Ganze Folge: H.264, Quelle angepasst, hohe Bitrate (YouTube).
2. Optional Clips 9:16: Sequenz duplizieren, Auto Reframe.
3. Vor dem Export einmal komplett überfliegen (Anfang, Ende, Schnitte, Ton).

## Regeln
- Nie Originaldateien löschen oder überschreiben, immer im Projekt arbeiten.
- Vor dem Export Nutzer kurz bestätigen lassen.
- Nach jedem Hauptschritt Projekt speichern (Cmd/Strg + S).
