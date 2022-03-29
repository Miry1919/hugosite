---
title: "Un promemoria per il futuro, caro GitHub"
date: 2022-03-29
---
Ieri alle ore 19:00 come ogni lunedì stavo cercando di pubblicare Tenero Gheriglio, aggiornando quindi la sua pagina (in particolare quella della [stagione 3](https://miry1919.github.io/hugosite/podcast/tenero-gheriglio-3/)) con una nuova puntata, la n° 75. Tuttavia sono incappata in un errore che mi si era già presentato tempo fa: nonostante secondo il terminale risultasse girare tutto nella norma, e mi restituisse "Everything-is-up-to-date", l'effettiva pubblicazione delle modifiche non avveniva affatto. Proprio perché questo problema mi si era già presentato, ma non di recente e raramente (una o due volte), avevo completamente dimenticato la soluzione, ai tempi cercata e trovata nella vasta marea di Internet, con le sue domande e risposte, Stack Overflow, Quora, Reddit e così via.

Per evitare di finire ancora una volta come ieri sera, insultarti male e voler lanciare il MacBook fuori dalla finestra dopo 77 tentativi non riusciti per risistemare tutto, oggi creiamo un promemoria per il futuro, per quando il tuo meccanismo si pianterà di nuovo senza motivo, caro GitHub.

&nbsp;

Se il classico codice non modifica effettivamente il sito:

1. effettuare una nuova modifica al .md in questione o a un .md a caso (da cancellare eventualmente in seguito);
2. ripartire coi seguenti comandi da terminale:

```
cd quickstart
hugo
git status
git init

/* inizializzazione che
** risolve tutto (!) */

git status
git add --all
git commit -m "podcast"
git push --force

/* comando 'git push --force'
** più efficace del semplice
** 'git push' */
```

3. fine.

&nbsp;

<div align="center">
  ✎
</div>
