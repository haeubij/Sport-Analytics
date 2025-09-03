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
- Nutzer können sich registrieren und anmelden
- Nutzer können Videos hochladen, verwalten und in Kategorien einordnen
- Nutzer können in Videos Markierungen und Laufwege einfügen
- Nutzer können eigene oder fremde Videos analysieren
- Geteilte Videos können kommentiert und bewertet werden
- Nutzer können bearbeitete Videos herunterladen
- Es gibt eine Benutzerverwaltung mit Rollen (z. B. Admin, Trainer, Spieler)

### Nicht-funktionale Anforderungen
- Die Web-App ist leicht verständlich und benutzerfreundlich aufgebaut
- Die Plattform ist responsive und läuft auf Desktop, Tablet und Smartphone
- Datenschutz wird beachtet, insbesondere bei Video-Uploads und Profilen
- Das System ist skalierbar – spätere Erweiterungen sind einfach möglich
- Die Applikation bietet eine stabile Performance auch bei größeren Videos
- Die Lösung ist wartbar durch eine modulare Struktur

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
