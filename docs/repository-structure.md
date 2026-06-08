# Repository Structure

## Ziel

Dieses Dokument beschreibt die Struktur des PlantQuest-Repositories.

Die Struktur soll das Projekt übersichtlich halten und zukünftige Erweiterungen erleichtern.

---

# Projektübersicht

```txt
plantquest/
├── app/
├── backend/
├── docs/
├── README.md
└── .gitignore
```

---

# app/

Der Ordner `app/` enthält die Mobile App.

Geplante Inhalte:

```txt
app/
├── screens/
├── components/
├── services/
├── hooks/
├── navigation/
├── assets/
└── types/
```

### Verantwortlichkeiten

* Benutzeroberfläche
* Navigation
* Formulare
* Pflanzenseiten
* Pflanzensammlung
* Kommunikation mit dem Backend

---

# backend/

Der Ordner `backend/` enthält den Serverteil der Anwendung.

Geplante Inhalte:

```txt
backend/
├── api/
├── services/
├── models/
├── database/
├── tests/
└── config/
```

### Verantwortlichkeiten

* Geschäftslogik
* API-Endpunkte
* Datenbankzugriffe
* Datenvalidierung
* spätere KI-Integration

---

# docs/

Der Ordner `docs/` enthält die Projektdokumentation.

Aktuelle Dokumente:

```txt
docs/
├── project-vision.md
├── user-stories.md
├── product-backlog.md
├── mvp-scope.md
├── architecture-overview.md
├── tech-stack.md
└── repository-structure.md
```

### Verantwortlichkeiten

* Planung
* Architektur
* Anforderungen
* Entscheidungen
* Projektdokumentation

---

# README.md

Die README-Datei dient als Einstiegspunkt für das Projekt.

Geplante Inhalte:

* Projektbeschreibung
* Funktionen
* Tech Stack
* Installation
* Projektstatus

---

# .gitignore

Die .gitignore-Datei definiert Dateien und Ordner, die nicht in Git gespeichert werden sollen.

Beispiele:

```txt
node_modules/
.env
__pycache__/
```

---

# Architekturprinzip

Die Projektstruktur folgt dem Prinzip der Trennung von Verantwortlichkeiten.

Jeder Ordner besitzt eine klar definierte Aufgabe.

Dadurch bleibt das Projekt:

* übersichtlich
* wartbar
* erweiterbar
* einfacher für neue Entwickler verständlich

```
```
