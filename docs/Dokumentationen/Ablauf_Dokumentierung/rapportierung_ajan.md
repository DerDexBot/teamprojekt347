# Rapportierung – 19:30 Uhr

**Datum / Zeit:** 19.09.2025 – 19:30  
**Teilnehmer:** Rudy (informiert), Ajan (informiert)  

## Inhalt
- Rudy hat Ajan über den bisherigen Stand des Projekts informiert.  
- Es wurden die bereits umgesetzten Punkte präsentiert:  
  - Erstellung der `docker-compose.yml`  
  - Aufsetzen und Testen der Services (MediaWiki, Nextcloud, Gogs, Portainer)  
  - Lösung technischer Probleme (Rechte, Ports, .env)  
  - Erstellung der Dokumentationsstruktur nach IPERKA  
  - Anfertigung von Arbeitsblättern und Gantt-Planung  
- Gemeinsame Absprache: Ajan übernimmt in der nächsten Phase ergänzende Dokumentationen und Tests.  

## Ergebnis
- Ajan ist nun auf dem gleichen Wissensstand.  
- Nächste Schritte können in der zweiten Arbeitssession gemeinsam fortgesetzt werden.  

---

# Kurzanleitung – Stand der Dinge

## 1. Projektstruktur
- Hauptordner `projekt_m347`  
- Unterordner: `docs/`, `volumes/`  
- Dateien: `docker-compose.yml`, `.env`, `.gitignore`, Dokumentationen (`.md`)  

## 2. Dienste
- MediaWiki → Port 8085, läuft mit MariaDB  
- Nextcloud → Port 8080, läuft mit MariaDB  
- Gogs → Standardport 3000, läuft mit MariaDB  
- Portainer → Port 9000  

## 3. Sicherheitsaspekte
- Passwörter nur in `.env` gespeichert  
- `.gitignore` verhindert Hochladen von sensiblen Daten  

## 4. Dokumentation
- IPERKA Gesamtdokumentation vorhanden  
- Arbeitsblätter 1–6 erstellt  
- Gantt-Planung als Übersicht + Details  

## 5. Status
- Alle Container getestet und lauffähig  
- Dokumentation teilweise nachträglich ergänzt, aber nun auf gutem Stand  
