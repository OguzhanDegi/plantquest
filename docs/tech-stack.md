# Tech Stack

## Ziel

Dieses Dokument beschreibt die Technologien, die für PlantQuest verwendet werden, sowie die Gründe für ihre Auswahl.

Die Auswahl orientiert sich an folgenden Zielen:

* moderne Softwareentwicklung lernen
* gute Portfolio-Wirkung
* Erweiterbarkeit
* große Community
* produktionsnahe Technologien

---

# Frontend

## React Native

React Native wird für die Entwicklung der mobilen App verwendet.

### Gründe für die Auswahl

* Entwicklung für Android und iOS mit einer Codebasis
* große Community
* weit verbreitet in Unternehmen
* gute Integration mit nativen Gerätefunktionen
* starke Unterstützung durch das React-Ökosystem

### Alternativen

* Flutter
* Native Android (Kotlin)
* Native iOS (Swift)

### Entscheidung

React Native bietet einen guten Kompromiss zwischen Lernaufwand, Marktverbreitung und Produktivität.

---

## Expo

Expo wird als Framework für React Native verwendet.

### Gründe für die Auswahl

* einfacher Projekteinstieg
* schnelle Entwicklung
* vereinfachter Zugriff auf Kamera und Gerätesensoren
* gute Entwicklererfahrung

### Alternativen

* React Native CLI

### Entscheidung

Für die frühe Entwicklungsphase ermöglicht Expo einen schnelleren und einfacheren Start.

---

## TypeScript

TypeScript wird als Programmiersprache im Frontend verwendet.

### Gründe für die Auswahl

* bessere Fehlererkennung
* bessere Wartbarkeit
* höhere Codequalität
* Industriestandard im modernen Frontend

### Alternativen

* JavaScript

### Entscheidung

TypeScript verbessert die Stabilität und Skalierbarkeit des Projekts.

---

# Backend

## Python

Python wird als Backend-Sprache verwendet.

### Gründe für die Auswahl

* leicht lesbar
* große Community
* ideal für spätere KI-Funktionen
* hohe Produktivität

### Alternativen

* Java
* C#
* JavaScript (Node.js)
* Go

### Entscheidung

Python passt besonders gut zu den langfristig geplanten KI-Funktionen.

---

## FastAPI

FastAPI wird als Backend-Framework verwendet.

### Gründe für die Auswahl

* moderne Architektur
* hohe Performance
* automatische API-Dokumentation
* gute Unterstützung von Type Hints

### Alternativen

* Flask
* Django

### Entscheidung

FastAPI bietet eine gute Balance zwischen Einfachheit und Professionalität.

---

# Datenbank

## PostgreSQL

PostgreSQL wird als relationale Datenbank verwendet.

### Gründe für die Auswahl

* Open Source
* weit verbreitet
* hohe Zuverlässigkeit
* gute Skalierbarkeit
* Industriestandard

### Alternativen

* MySQL
* SQLite
* MongoDB

### Entscheidung

PostgreSQL eignet sich gut für langfristiges Wachstum und professionelle Anwendungen.

---

# Versionsverwaltung

## Git

Git wird für die Versionsverwaltung verwendet.

Aufgaben:

* Änderungen nachvollziehen
* Versionen verwalten
* Zusammenarbeit ermöglichen

---

## GitHub

GitHub wird als zentrale Plattform für das Repository verwendet.

Aufgaben:

* Quellcodeverwaltung
* Dokumentation
* Portfolio-Präsentation
* spätere CI/CD-Integration

---

# Zukünftige Technologien

Folgende Technologien sind aktuell nicht Bestandteil von MVP 0.1, können jedoch später ergänzt werden:

## KI

Mögliche Optionen:

* OpenAI
* Gemini
* PlantNet
* Plant.id

---

## Containerisierung

Mögliche Technologie:

* Docker

---

## Authentifizierung

Mögliche Technologien:

* JWT
* OAuth 2.0

---

# Zusammenfassung

Der aktuelle Tech Stack für PlantQuest:

```txt
Frontend
- React Native
- Expo
- TypeScript

Backend
- Python
- FastAPI

Datenbank
- PostgreSQL

Versionsverwaltung
- Git
- GitHub
```
