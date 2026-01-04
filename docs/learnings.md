\## Issue 1 – Erste API



\*\*Endpoint:\*\* https://jsonplaceholder.typicode.com/todos  

\*\*Methode:\*\* GET  

\*\*Parameter:\*\* userId=1  

\*\*Statuscode:\*\* 200



\### Was bedeutet das?

\- Ich frage eine Liste von Todos ab und filtere nach userId=1.



\### JSON erklärt

\- `\[]` = Array (Liste)

\- `{}` = Objekt (ein Eintrag)

\- Beispiel-Felder:

&nbsp; - `userId` (Number): Nutzer-ID

&nbsp; - `title` (String): Titel

&nbsp; - `completed` (Boolean): true/false




## Issue 2 – Statuscodes 400 vs. 404

**404 Not Found**
- Beispiel: GET https://jsonplaceholder.typicode.com/todos/999999
- Bedeutung: Adresse/Ressource existiert nicht.

**400 Bad Request**
- Beispiel: GET https://httpbin.org/status/400
- Bedeutung: Anfrage ist syntaktisch/inhaltlich ungültig.

**200 OK**
- Beispiel: GET https://jsonplaceholder.typicode.com/todos?userId=1
- Bedeutung: Anfrage korrekt, Daten geliefert.
