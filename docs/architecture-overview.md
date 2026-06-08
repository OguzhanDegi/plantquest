# Architecture Overview

## Zweck dieses Dokuments

Dieses Dokument beschreibt die technische Gesamtarchitektur von PlantQuest.

Es dient als zentrale Übersicht über die wichtigsten Systemkomponenten, deren Verantwortlichkeiten und die Kommunikation zwischen ihnen.

Die Architektur soll bewusst einfach starten und schrittweise erweitert werden können.

---

# Systemübersicht

PlantQuest besteht aus mehreren voneinander getrennten Komponenten.

```txt
Mobile App
    ↓
Backend API
    ↓
Datenbank
```

In späteren Versionen wird die Architektur erweitert:

```txt
Mobile App
    ↓
Backend API
    ↓
Datenbank

Backend API
    ↓
KI-Service
```

---

# Komponenten

## Mobile App (Frontend)

Die Mobile App ist die Benutzerschnittstelle des Systems.

Repository:

```txt
app/
```

Verantwortlichkeiten:

* Pflanzen erfassen
* Fotos aufnehmen oder auswählen
* Formulare anzeigen
* Pflanzenseiten darstellen
* Pflanzensammlung anzeigen
* Daten an das Backend senden
* Daten vom Backend empfangen

Geplante Technologien:

* Expo
* React Native
* TypeScript

---

## Backend API

Das Backend enthält die Geschäftslogik der Anwendung.

Repository:

```txt
backend/
```

Verantwortlichkeiten:

* Pflanzendaten verarbeiten
* Daten validieren
* Pflanzen speichern
* Pflanzen abrufen
* Datenbankzugriffe verwalten
* spätere KI-Funktionen integrieren

Geplante Technologien:

* Python
* FastAPI

---

## Datenbank

Die Datenbank speichert alle persistenten Daten.

Geplante Technologie:

* PostgreSQL

Geplante Daten einer Pflanze:

```txt
id
name
description
image_url
created_at
updated_at
```

---

## KI-Service (zukünftige Erweiterung)

Der KI-Service ist nicht Bestandteil von MVP 0.1.

Geplante Aufgaben:

* Pflanzenerkennung anhand von Bildern
* automatische Erstellung von Pflanzeninformationen
* KI-Chat
* Erweiterung bestehender Pflanzenseiten

---

# Kommunikation zwischen den Komponenten

Die Mobile App kommuniziert ausschließlich mit dem Backend.

Die Datenbank ist niemals direkt von der App erreichbar.

```txt
App
 ↓
Backend
 ↓
Datenbank
```

Vorteile:

* bessere Sicherheit
* zentrale Geschäftslogik
* einfachere Erweiterbarkeit
* austauschbare Datenbanktechnologien

---

# Datenfluss in MVP 0.1

Der geplante Ablauf für MVP 0.1:

```txt
1. Nutzer erstellt ein Pflanzenfoto.
2. Nutzer gibt Name und Beschreibung ein.
3. App sendet die Daten an das Backend.
4. Backend verarbeitet die Anfrage.
5. Backend speichert die Pflanze.
6. Datenbank speichert die Informationen.
7. App lädt die gespeicherten Pflanzen.
8. Nutzer sieht die Pflanzensammlung.
```

---

# Architekturprinzipien

Für PlantQuest gelten folgende Grundsätze:

* einfache Architektur vor komplexer Architektur
* klare Trennung von Frontend und Backend
* Erweiterbarkeit für zukünftige KI-Funktionen
* MVP zuerst, Optimierung später
* schrittweiser Ausbau statt Überentwicklung

---

# Aktueller Stand

Aktuell befindet sich PlantQuest in MVP 0.1.

Folgende Funktionen sind Bestandteil des MVP:

* Pflanze erfassen
* Pflanzenseite anzeigen
* Pflanze speichern
* Pflanzensammlung anzeigen

KI-Funktionen, Community-Funktionen und Gamification sind derzeit nicht Bestandteil der Architektur.
