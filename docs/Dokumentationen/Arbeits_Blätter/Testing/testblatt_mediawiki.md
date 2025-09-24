# Arbeitsblatt – Testing Nextcloud

**ID:** Test-2  
**Service:** Nextcloud (Port 8080)  
**Datum:** …  
**Verantwortlich:** Ajan

---

## Testziele
- Sicherstellen, dass Nextcloud für Filesharing funktioniert.

## Testschritte
1. Browser öffnen → `http://localhost:8080`.
2. Mit Default-User einloggen.
3. Testdatei (`test.txt`) hochladen.
4. Datei herunterladen und Inhalt prüfen.
5. Container neustarten → prüfen, ob Datei noch vorhanden ist.

## Erwartetes Ergebnis
- Oberfläche erreichbar.
- Datei kann hoch- und heruntergeladen werden.
- Datei bleibt nach Neustart vorhanden.

## Ergebnis
- [ ] OK
- [ ] Fehler (Beschreibung hier eintragen)  