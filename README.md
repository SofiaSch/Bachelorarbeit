# LaTeX-Framework: Bachelorarbeit Sofia Schepers

Dieses Repository enthält das LaTeX-Schreibskript und die Dokumentenstruktur für die Bachelorarbeit:
**"Verfahrensdauer und Wettbewerb in der öffentlichen Auftragsvergabe: Eine vergleichende Analyse der Effekte auf die Gesamt- und KMU-Beteiligung in Deutschland, Estland und Frankreich"**

Eingereicht an der **Technischen Universität München (TUM)**, Chair for Strategy and Organization.

## 📁 Repository-Struktur

Das Projekt ist modular aufgebaut, um eine saubere Trennung von Inhalt, Logik und Ressourcen zu gewährleisten:

* `main.tex`: Die zentrale Hauptdatei, die alle Pakete lädt und die Sektionen zusammenführt.
* `bibliothek.bib`: Die Literaturdatenbank im BibLaTeX-Format (APA-Stil).
* `sections/`: Enthält die einzelnen Kapitel der Arbeit (`00_cover.tex` bis `11_erklaerung.tex`).
* `images/`: Enthält alle Abbildungen, Diagramme (Interaktionseffekte, Boxplots) und Logos.
* `requirements.txt`: Dokumentiert die für die Skriptumgebung (z.B. Automatisierungstools) genutzten Versionen.

## 🛠 Setup & Kompilierung

Dieses Projekt nutzt `pdflatex` zur PDF-Generierung und `biber` für das Literaturmanagement (APA 7th Edition).

### Voraussetzungen
Stellen Sie sicher, dass eine aktuelle TeX-Distribution (z. B. TeX Live 2025 oder MiKTeX) installiert ist.

### Kompilier-Reihenfolge
Um alle Querverweise, das Inhaltsverzeichnis und das Literaturverzeichnis korrekt zu generieren, führen Sie folgende Befehle aus:

1. `pdflatex main.tex`
2. `biber main`
3. `pdflatex main.tex`
4. `pdflatex main.tex`

## 📝 Lizenz und Transparenz
Dieses Repository dient der Dokumentation des Schreibprozesses und der Sicherstellung der wissenschaftlichen Replizierbarkeit der Formatierung. Der inhaltliche Kern der statistischen Analyse befindet sich in einem separaten Repository (siehe Anhang A5 der Arbeit).