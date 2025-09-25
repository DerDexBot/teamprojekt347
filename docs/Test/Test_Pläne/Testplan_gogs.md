# Testplan – Testing Gogs

**ID:** Test-3  
**Service:** Gogs (Port 3000)  
**Datum:** …  
**Verantwortlich:** Ajan

---

## Testziele
- Sicherstellen, dass Gogs als Git-Service funktioniert.

## Testschritte
1. Browser öffnen → `http://localhost:3000`.
2. Admin-User anlegen.
3. Neues Repository erstellen (`demo-repo`).
4. Auf lokalem Rechner Repo klonen:
   ```bash
   git clone http://localhost:3000/ajan/demo-repo.git