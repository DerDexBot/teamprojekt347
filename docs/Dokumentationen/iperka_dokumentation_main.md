```
IPERKA Gesamtdokumentation – Projekt Container-Services
1. Informieren

Ausgangslage:

Ein KMU möchte firmeninterne Services in Containern bereitstellen.

Gefordert sind:
•   MediaWiki (Port 8085) für interne Dokumentation
•   Nextcloud (Port 8080) für Filesharing
•   Gogs für Quellcodeverwaltung (Alternative zu GitLab wegen Ressourcen)
•   Portainer zur Überwachung

Alle Daten müssen persistent gespeichert werden.
Projektzeit: 2×4 Lektionen = 8 Lektionen ( 8 Stunden).

Infrastruktur: Ubuntu-VM (8GB RAM, 50GB HDD), Docker und Compose, GitHub für Versionierung.

Erkenntnis: Die zentrale Herausforderung liegt weniger in der Technik, sondern in der Planung, Dokumentation und Nachvollziehbarkeit.
## 2. Planen



**Detailzeitplanung (Phasen im Block 1):**
|---------------|---------|--------|-------|
| Phase         | Start   | Ende   | Dauer |
|---------------|---------|--------|-------|
| Informieren   | 13:00   | 13:15  | 0.25h |
| Planen        | 13:15   | 13:45  | 0.5h  |
| Entscheiden   | 13:45   | 14:15  | 0.5h  |
| Realisieren   | 14:15   | 15:30  | 1.25h |
| Kontrollieren | 15:30   | 15:55  | 0.42h |
| Auswerten     | 15:55   | 16:15  | 0.33h |
|---------------|---------|--------|-------|

**Aufgabenteilung:** Da Partner krank war → alle Schritte von Lernendem *Rudy* durchgeführt.

3. Entscheiden
Architekturentscheidungen:
Alle Dienste in einem zentralen docker-compose.yml
Netzwerk: gemeinsames internes Bridge-Netzwerk
Volumes: unter volumes/ pro Service
Datenbank je für MediaWiki, Nextcloud, Gogs
.env zur Geheimhaltung von Passwörtern

Testkonzept:
•   Nextcloud: Datei hochladen und herunterladen
•   MediaWiki: Seite anlegen und speichern
•   Gogs: Repo erstellen, Push/Pull testen
•   Portainer: Überwachung aller Container

Sicherheitskonzept:
Keine Passwörter im Compose-File
.gitignore verhindert Upload von .env und Volumes
Nur benötigte Ports freigegeben
Ressourcengrenzen (Option für Erweiterung)
 

4. Realisieren
Projektordner projekt_m347 erstellt
docker-compose.yml geschrieben mit Services:
•   MediaWiki + MariaDB
•   Nextcloud + MariaDB
•   Gogs + MariaDB
•   Portainer
•   .env Datei mit allen Zugangsdaten angelegt
•   .gitignore erstellt (ignoriert .env und Volumes
•   Container gestartet mit docker compose up -d 
Probleme gelöst:
•   Rechteproblem bei MediaWiki (Volumes angepasst)
•   Portainer-Konflikt mit altem Container (Container gelöscht, neu gestartet)
5. Kontrollieren
Abgleich mit Planung:
•   Technisch: alle Dienste laufen stabil und sind über Browser erreichbar
•   Zeit: mehr Aufwand beim Realisieren, weniger bei Dokumentation
•   Tests durchgeführt → Ergebnisse protokolliert
•   GitHub-Repo gepflegt mit Commits und Projektstruktur
Abweichungen:
•   Dokumentation zu spät begonnen → musste nachträglich erstellt werden
•   Planung (Gantt, Journal) erst im Nachhinein vervollständigt
 

6. Auswerten
Lernerfahrungen:
•   Technisch: Umgang mit docker-compose, Service-Vernetzung, Portainer, GitHub
•   Organisatorisch: Dokumentation und Planung sind genauso wichtig wie die Technik
•   Probleme: Rechte bei Volumes, Portainer-Doppelung
•   Verbesserung: Nächstes Mal IPERKA konsequent von Beginn an dokumentieren

Fazit: Projektziel wurde technisch erreicht: Alle Dienste laufen in Containern und sind persistent gespeichert. GitHub-Repo dokumentiert die Arbeit. Dokumentation war anfänglich mangelhaft, wurde aber nachgearbeitet. Gesamt: Projekt erfolgreich, mit Verbesserungspotenzial in Planung/Dokumentation.
```