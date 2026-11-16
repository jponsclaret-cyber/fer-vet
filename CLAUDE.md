# fer-vet (instruccions per a Claude)

Repositori **públic** d'un projecte per a un client: tot el que hi hagi, historial inclòs, és públic.

## Seguretat (mode estricte)

- Abans de fer commit o push, i en acabar qualsevol canvi, aplica la revisió de seguretat (la skill `revisio-seguretat`
  si la tens; si no, aquesta llista).
- **Cap dada real dels clients del client, cap secret, clau ni fitxer de dades** al repositori ni a la conversa
  (`*.xlsx`, `*.csv`, `fervert_db*.json`…). Proves només amb dades inventades. El `.gitignore` ja els exclou: no el relaxis.
- Les pàgines són estàtiques i treballen amb les dades al navegador. No afegeixis serveis externs ni scripts de tercers
  sense preguntar, i cap script sense versió fixada i `integrity`. Cada pàgina té una política de contingut (CSP) a la
  capçalera que limita a quins serveis es pot connectar: si canvia algun servei, actualitza-la i prova la pàgina.
- Als serveis externs només hi poden anar coordenades i textos de cerca (ICGC, OSRM, REGA): mai noms ni dades personals.
- Tot el que s'insereix com a HTML s'escapa amb `esc()`.
- No canviïs la visibilitat del repositori ni publiquis res nou sense preguntar a en Jimix.
