# Testplan – MediaWiki

**ID:** Test-1  
**Service:** MediaWiki (Port 8085)  
**Datum:** …  
**Verantwortlich:** Ajan

---

## Testziele
- Sicherstellen, dass MediaWiki erreichbar ist und Inhalte persistent gespeichert werden.

## Testschritte
1. Browser öffnen → `http://localhost:8085`
2. Login (falls erforderlich) überspringen → Hauptseite aufrufen.
3. Neue Seite anlegen → Inhalt speichern.
4. MediaWiki Container löschen und neu starten mit dem Befehl: docker rm mediawiki, docker compose up -d --build
5. Seite erneut öffnen → prüfen, ob Inhalt persistiert ist.

## Erwartetes Ergebnis
- Startseite von MediaWiki ist erreichbar.
- Neue Seite lässt sich speichern und aufrufen.
- Daten bleiben nach Container-Neustart bestehen (Volume-Test).

## Ergebnis
- [ ] OK
- [ ] Fehler (Beschreibung hier eintragen)  