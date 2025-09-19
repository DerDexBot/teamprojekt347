# Rapportierung – Umgang mit Links in GitHub Markdown

**Datum / Zeit:** 19.09.2025 – 20:10 bis 20:50  
**Dauer:** ca. 40 Minuten  
**Teilnehmer:** Rudy

---

## Inhalt
- Fehler bei internen Verlinkungen in der Dokumentation (`.md`-Dateien) analysiert.
- Ursache: falsche relative Pfade und Sonderzeichen (Umlaut „ä“) im Ordnernamen `Arbeits_Blätter`.
- Vorgehen:
    - Pfadstruktur genau geprüft und nachvollzogen.
    - Ordnername in `Arbeits_Blaetter` umbenannt, um GitHub-kompatible Links zu ermöglichen.
    - Alle Verlinkungen in `iperka_dokumentation_main.md` angepasst → relative Pfade korrekt gesetzt.
    - Anschließend getestet: Alle Links funktionieren nun auf GitHub ohne 404-Fehler.

---

## Ergebnis
- Verständnis aufgebaut, wie **Markdown-Links** und **relative Pfade** in GitHub funktionieren.
- Wichtig gelernt:
    - Pfade müssen exakt der Ordnerstruktur entsprechen (inkl. Groß-/Kleinschreibung).
    - Sonderzeichen in Ordnernamen (z. B. Umlaute) können Probleme verursachen → besser vermeiden.
    - Änderungen an Pfaden immer auch in den Verlinkungen nachziehen.

---

## Nächste Schritte
- Weitere Dokumentationen und Arbeitsblätter konsequent mit relativen Links verknüpfen.
- Bei zukünftigen Anpassungen an der Struktur sofort im Arbeitsjournal dokumentieren.  
