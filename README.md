# SportAnalytics – Webbasierte Videoanalyse für Amateursport

## Projektbeschreibung

SportAnalytics ist eine webbasierte Plattform zur Videoanalyse, die speziell für Amateursportler, Trainer, Vereine und Sportbegeisterte entwickelt wurde. Während professionelle Teams teure Softwarelösungen nutzen, zielt dieses Projekt darauf ab, eine kostenlose, intuitive und sportartenübergreifende Alternative bereitzustellen.

## Projektziele (nicht-technisch)

1. Zugang zur Videoanalyse für alle ermöglichen  
Sportanalyse darf kein Privileg für Profis sein. Mit dieser Plattform sollen auch Amateursportler, Schulsportlehrer und Vereine moderne Analysemöglichkeiten erhalten – kostenlos und ohne technische Hürden.

2. Sportartenübergreifende Nutzung  
Die Plattform soll nicht auf eine bestimmte Sportart beschränkt sein. Ob Fußball, Volleyball, Leichtathletik oder Schulsport – jede Disziplin soll profitieren.

3. Eigenständiges Lernen und Reflexion fördern  
Durch Analysefunktionen wie Markierungen oder Laufwege können Sportler ihr eigenes Spielverhalten nachvollziehen, Fehler erkennen und gezielt daran arbeiten.

4. Austausch und Zusammenarbeit ermöglichen  
Über eine integrierte Community-Funktion können Videos geteilt, kommentiert und bewertet werden – so entsteht ein Raum für Wissenstransfer und sportlichen Austausch.

5. Einfache und intuitive Bedienung  
Die Plattform wird so gestaltet, dass sie auch ohne technisches Vorwissen verständlich ist – klar strukturiert, logisch aufgebaut und einfach zu bedienen.

6. Nutzung von überall  
Durch die Web-Technologie ist die Nutzung auf allen Geräten möglich – egal ob Desktop, Tablet oder Smartphone, zu Hause oder auf dem Spielfeld.

## Anforderungen an die Applikation

### Funktionale Anforderungen
- 1. Nutzer können sich registrieren und anmelden
- 2. Nutzer können Videos hochladen, verwalten und in Kategorien einordnen
- 3. Nutzer können in Videos Markierungen und Laufwege einfügen
- 4. Nutzer können eigene oder fremde Videos analysieren
- 5. Geteilte Videos können kommentiert und bewertet werden
- 6. Nutzer können bearbeitete Videos herunterladen
- 7. Es gibt eine Benutzerverwaltung mit Rollen (z. B. Admin, Trainer, Spieler)

### Nicht-funktionale Anforderungen
- 1. Die Web-App ist leicht verständlich und benutzerfreundlich aufgebaut
- 2. Die Plattform ist responsive und läuft auf Desktop, Tablet und Smartphone
- 3. Datenschutz wird beachtet, insbesondere bei Video-Uploads und Profilen
- 4. Das System ist skalierbar – spätere Erweiterungen sind einfach möglich
- 5. Die Applikation bietet eine stabile Performance auch bei größeren Videos
- 6. Die Lösung ist wartbar durch eine modulare Struktur

## Probleme, die gelöst werden

- Hohe Einstiegshürden durch professionelle Tools  
  → SportAnalytics ist kostenlos und barrierefrei.

- Komplizierte oder überladene Software  
  → Die Anwendung ist bewusst einfach und verständlich gehalten.

- Fehlende zentrale Plattform für Analyse und Austausch  
  → SportAnalytics bietet eine gemeinsame Umgebung für Trainer und Spieler.

- Isoliertes Arbeiten im Amateurbereich  
  → Mit der Community-Funktion wird gegenseitige Unterstützung und Lernen gefördert.

- Technische Hürden (Installation, Lizenzen etc.)  
  → Kein Installationsaufwand: läuft direkt im Browser.

## Zielgruppe

- Amateursportler und -vereine  
- Trainer im Nachwuchsbereich  
- Sportunterricht an Schulen  
- Sportanalysten im nicht-professionellen Umfeld  
- Sportbegeisterte, die ihr Spiel verbessern möchten

## Architektur und Technologie (kurz)

- Frontend: Angular (v19)
- Backend: Node.js mit Express
- Datenbank: MongoDB
- Authentifizierung: JWT
- Speicherung: Lokales Dateisystem oder optional Cloud (z. B. AWS S3)


# SportAnalytics User Stories

## Aktuelle User Stories (Statusübersicht)

### User Story 1: Video-Upload & Kategorisierung
- **Als** Nutzer
- **möchte ich** Videos hochladen und in Kategorien organisieren,
- **damit ich** verschiedene Spielszenen besser strukturieren kann.

**Akzeptanzkriterien:**
- Der Nutzer kann ein Video hochladen.
- Der Nutzer kann eine Sportart oder Kategorie auswählen.
- Das Video wird korrekt zugeordnet angezeigt.

**Status:** Teilweise umgesetzt  
**To-do:** Kategorisierungsfunktion fehlt noch

---

### User Story 2: Markierungen & Laufwege einfügen
- **Als** Trainer
- **möchte ich** Markierungen und Laufwege in Videos einfügen,
- **damit ich** Spielsituationen für meine Spieler analysieren kann.

**Akzeptanzkriterien:**
- Nutzer kann Marker, Kreise und Pfeile setzen.
- Markierungen bleiben gespeichert.
- Optional: Zeitlich synchronisiert mit Video.

**Status:** Noch nicht begonnen  
**To-do:** Technische Machbarkeit prüfen (Canvas/SVG Overlay)

---

### User Story 3: Videos mit der Community teilen
- **Als** Nutzer
- **möchte ich** bearbeitete Videos öffentlich teilen,
- **damit ich** Feedback oder Inspiration erhalten kann.

**Akzeptanzkriterien:**
- Videos können als „öffentlich“ markiert werden.
- Sie erscheinen im Community-Bereich.

**Status:** Umgesetzt

---

### User Story 4: Bearbeitete Videos herunterladen
- **Als** Nutzer
- **möchte ich** bearbeitete Videos herunterladen,
- **damit ich** sie offline oder extern verwenden kann.

**Akzeptanzkriterien:**
- Video inklusive Markierungen kann heruntergeladen werden.
- Downloadformat ist gebräuchlich (z. B. MP4).

**Status:** Umgesetzt

---

### User Story 5: Kommentare & Bewertungen
- **Als** Nutzer
- **möchte ich** Videos kommentieren und bewerten,
- **damit ich** mich mit anderen Nutzern austauschen kann.

**Akzeptanzkriterien:**
- Kommentarfunktion unter Videos verfügbar.
- Bewertung (z. B. Sterne) ist möglich.
- Speicherung & Anzeige der Inhalte.

**Status:** Noch nicht umgesetzt  
**To-do:** Kommentarmodell, API und Frontend-Komponente entwickeln

---

## Erweiterungsideen für zukünftige Releases

### Erweiterte Analysefunktionen
- Zeitmarken mit Annotationen
- Manuelle Heatmap-Funktion durch Nutzerinteraktion
- KI-gestützte Erkennung (z. B. Spielerpositionen, Tore)

### Community- und Social-Features
- Favoriten und Like-Funktion
- Öffentliche Profile mit Statistiken
- Folgen-Funktion für Nutzer

### Funktionen für Teams & Trainer
- Gruppen- und Teamverwaltung
- Übungssammlung mit Trainingsvideos
- Aufgaben und Analyseaufträge für Spieler

### Technische Verbesserungen
- Progressive Web App (PWA)
- Push-Benachrichtigungen
- Drag & Drop Upload im Frontend

### Sicherheit & Benutzerrollen
- Zwei-Faktor-Authentifizierung (2FA)
- Erweiterte Rollen (z. B. Co-Trainer, Analyst)
- Private Gruppen für geschützte Inhalte

### Monitoring & Feedback
- Interne Feedbackfunktion für Nutzer
- Admin-Dashboard mit Statistiken
- Watchtime- und Engagement-Analyse

---

## Nächste Schritte (Vorschlag)

1. Umsetzung der Kommentarfunktion (Story 5)
2. Einführung eines Favoriten-/Like-Systems
3. Entwicklung von Nutzerprofilen mit Statistiken

Diese drei Punkte bilden die Basis für mehr Interaktion, Feedback und Nutzerbindung.

---

## Lizenz & Hinweise

Dieses Projekt ist Teil eines schulischen Projekts im Rahmen des Moduls 306 und nicht öffentlich lizenziert. Die Nutzung erfolgt ausschließlich zu Ausbildungszwecken.




## Weitere Informationen

Für technische Details (Architektur, Komponenten, APIs, Datenmodelle etc.), siehe bitte die Datei `SportAnalytics_Zusammenfassung.txt` oder die UML-Diagramme im Projektverzeichnis.

## Kontakt & Mitwirkung

Dieses Projekt wurde im Rahmen des Moduls 306 an der GIBB Bern umgesetzt. Wir freuen uns über Feedback, Vorschläge oder Beiträge.

Projektteam:  
Janis Häubi, Manuel Affolter, Pascal Fankhauser, Levin Keller






# Analyse der Komponentenabhängigkeiten im Auslieferungsprozess  

## Übersicht
Dieses Dokument beschreibt die Abhängigkeiten der Komponenten der SportAnalytics-Webapplikation und deren Auswirkungen auf den Auslieferungs- und Deployment-Prozess.  
Die Anwendung besteht aus einem Angular-Frontend, einem Node.js-Backend, einer MongoDB-Datenbank sowie einem lokalen Video-Upload-System.

## Systemkomponenten

### 1. Frontend (Angular)
- Stellt die Benutzeroberfläche bereit  
- Kommuniziert über REST-API mit dem Backend  
- Wird als statisches Build-Paket ausgeliefert (z. B. Webserver)

### 2. Backend (Node.js)
- API-Server mit Geschäftslogik  
- Verarbeitung von Video-Uploads und Nutzeraktionen  
- JWT-Authentifizierung  
- Benötigt aktive Datenbankverbindung

### 3. Datenbank (MongoDB)
- Speicherung von Nutzern, Videometadaten und Berechtigungen  
- Muss vor dem Backend laufen, da das Backend beim Start eine Verbindung herstellt

### 4. Videospeicher (lokales Upload-Verzeichnis)
- Speicherort der hochgeladenen Video-Dateien  
- Backend benötigt Schreib-/Leserechte für das Verzeichnis `uploads/`

## Abhängigkeiten zwischen den Komponenten

### Frontend → Backend
- Das Frontend ist vollständig auf eine funktionierende API angewiesen  
- Änderungen an API-Endpunkten müssen im Frontend angepasst werden  
- Fehlerhafte API-URL im `environment.ts` führt zu Funktionsausfällen

### Backend → Datenbank
- Das Backend kann ohne aktive Datenbank nicht starten  
- Datenmodelländerungen erfordern eine abgestimmte Backend-Version  
- Fehlerhafte MongoDB-URI oder nicht laufender Dienst blockieren das Deployment

### Backend → Videospeicher
- Das Verzeichnis `uploads/` muss existieren  
- Fehlende Schreibrechte verhindern Video-Uploads  
- Backend muss Zugriffspfad korrekt konfiguriert haben

## Ablauf des Auslieferungsprozesses

1. Start der MongoDB-Datenbank  
2. Starten des Backends (API wird bereitgestellt)  
3. Build und Deployment des Frontends  
4. Überprüfung des Upload-Verzeichnisses und der Berechtigungen  

Jede Komponente ist notwendige Voraussetzung für den nächsten Schritt. Fehler im Ablauf führen zu Ausfällen im Gesamtsystem.

## Risiken und Herausforderungen

| Risiko | Beschreibung | Auswirkung |
|--------|--------------|------------|
| Nicht erreichbare Datenbank | MongoDB läuft nicht oder fehlerhafte URI | Backend startet nicht |
| Falsche API-URL im Frontend | Konfigurationsfehler in `environment.ts` | Login, Upload und Community-Funktionen fallen aus |
| Versionskonflikte | Änderungen im Backend ohne Anpassungen im Frontend | Fehlende oder fehlerhafte Daten |
| Rechteprobleme im Upload-Verzeichnis | Schreibrechte fehlen | Uploads schlagen fehl |

## Massnahmen zur Risikominimierung
- Verwendung von `.env`-Dateien für Backend-Konfiguration  
- Klare Versionierung der API und Datenmodelle  
- Automatisierte Tests zur Überprüfung der API-Kompatibilität  
- Deploy-Skripte, die die Verfügbarkeit von MongoDB prüfen  
- Dokumentation aller Änderungen an Schnittstellen und Datenmodellen  

## Fazit
Die Analyse zeigt, dass ein stabiler Auslieferungsprozess nur durch abgestimmtes Zusammenspiel aller Komponenten gewährleistet werden kann. Besonders kritisch sind die Abhängigkeiten zwischen Datenbank, Backend und Frontend. Durch strukturierte Konfiguration, getestete Deployment-Abfolgen und saubere Dokumentation können typische Fehlerquellen vermieden werden.

---

## 7. Best Practices für Integration und Prozessdokumentation (Kurzfassung)

### Zweck

Dieses Kapitel beschreibt einfache, verbindliche Regeln für Integration, Deployment und Qualitätssicherung von **SportAnalytics**. Ziel ist ein stabiler Betrieb mit klaren Abläufen und möglichst wenig Komplexität.

Geltungsbereich:

* Angular Frontend
* Node.js + Express Backend
* MongoDB
* JWT Authentifizierung

---

### Projektstruktur (vereinfacht)

```
project-root/
├── frontend/    # Angular
├── backend/     # Node.js / Express
├── docs/        # Dokumentation
├── scripts/     # Deploy- & Check-Skripte
└── .github/     # CI (optional)
```

Grundregel: Frontend, Backend und Datenbank sind klar getrennt und kommunizieren nur über REST-APIs.

---

### Deployment-Prozess (Kurz)

Reihenfolge:

1. MongoDB starten
2. Backend starten
3. Backend Health-Check
4. Frontend builden und deployen
5. Kurzer Funktionstest

Minimal-Checks:

* API erreichbar (`/health` → ok)
* Frontend lädt
* Upload-Verzeichnis beschreibbar

---

### Umgebungskonfiguration

* **Keine Secrets im Code**
* Konfiguration über `.env`
* `.env.example` als Vorlage im Repository

Wichtige Variablen:

* `MONGODB_URI`
* `JWT_SECRET`
* `NODE_ENV`
* `UPLOAD_DIR`

Fehlende Variablen müssen den Start abbrechen.

---

### Abhängigkeiten

* Frontend benötigt laufendes Backend
* Backend benötigt laufende MongoDB
* Upload-Funktion benötigt Schreibrechte

Bei Fehlern: zuerst Datenbank, dann Backend, zuletzt Frontend prüfen.

---

### Versionskontrolle

* `main`: stabile Version
* `feature/<name>`: neue Funktionen
* `bugfix/<name>`: Fehlerbehebungen

Commits klar und kurz:

* `feat: Video Upload`
* `fix: Login Fehler`
* `docs: API angepasst`

Versionierung nach SemVer (z. B. 1.0.0 → 1.1.0 → 1.1.1).

---

### Testing (Minimalstandard)

* Unit Tests für zentrale Logik
* API-Tests für wichtigste Endpunkte
* Nach Deployment: Smoke-Test (Login, Videoübersicht, Upload)

Ziel: Fehler früh erkennen, nicht perfekte Testabdeckung.

---

### CI/CD (optional)

* Automatische Tests bei Push oder Pull Request
* Merge in `main` nur bei erfolgreichen Tests
* Deployment kann manuell oder automatisiert erfolgen

---

### Kernaussage

Klare Trennung der Komponenten, einfache Deploy-Reihenfolge, saubere Konfiguration und minimale Tests reichen aus, um SportAnalytics stabil, nachvollziehbar und erweiterbar zu betreiben.

