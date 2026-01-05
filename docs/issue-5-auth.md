# Issue 5 – Authentifizierung

## Ziel

Auth Basics verstehen und praktisch testen: Token, Authorization-Header, 401 vs 403.

## Setup

* Tool: Postman
* Repo: api-basics-lab
* Issue: https://github.com/tobiknoke-oss/api-basics-lab/issues/5

## Tests (Beobachtung)

### A) No Token (erwartet: 401)

* Request (Methode + URL):
* Auth-Setup (Postman):
* Ergebnis (Statuscode):
* Response-Hinweis (1 Satz):
* Interpretation:

### B) Invalid Token (erwartet: 401 oder 403)

* Request (Methode + URL):
* Auth-Setup (Postman):
* Ergebnis (Statuscode):
* Response-Hinweis (1 Satz):
* Interpretation:

### C) Valid Token (erwartet: 200/201 oder 403)

* Request (Methode + URL):
* Auth-Setup (Postman):
* Ergebnis (Statuscode):
* Response-Hinweis (1 Satz):
* Interpretation:
* A) No Token
* 
* Ergebnis: 401 Unauthorized
* 
* Interpretation: Kein Auth-Nachweis ? Zugriff verweigert
* 
* B) Bearer INVALID\_TOKEN
* 
* Ergebnis: 200 OK
* 
* Interpretation: API prüft nur Header-Präsenz, nicht Token-Gültigkeit
* 
* C) Bearer abc123
* 
* Ergebnis: 200 OK
* 
* Interpretation: Bearer-Header vorhanden ? Request akzeptiert
* 
* Kurzfazit (Pflicht, wie bei Issue 1–4):
* 
* 401 = nicht authentifiziert
* 
* 403 = authentifiziert, aber nicht autorisiert (bei echten APIs)
* 
* Statuscodes sind API-Implementierungsentscheidungen
