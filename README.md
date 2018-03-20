# User Tracking
L'applicazione è stata sviluppata da:

* Stefano Baruffa
* Marco Pavia

## Introduzione
Questo progetto è una piattaforma realizzata interamente in JavaScrispt e HTML, e utilizza un database NoSQL Firebase. Lo scopo è quello di profilare gli utenti che vi accedono e di raccogliere informazioni riguardanti il comportamnto utente utili per l'analisi di mercato e la loro profilazione. È stato necessario creare un dominio adatto al contesto della profilazione, un dominio in grado di catturare l'attenzione dell'utente e che gli permettesse di poter osservare dei contenuti e di poter prendere delle decisioni.

La struttura del progetto è la seguente:
* index.html: è la pagina principale tramite la quale l'utente accede al servizio. In particolare se è il primo accesso, allora l'utente può inserire nome, cognome e scegliere la tecnica di tracciamento e portato alla pagina images.html; in caso contrario l'utente sarà riconosciuto e re-indirizzato automaticamente alla pagina return.html.
* return.html: è la pagina di benvenuto, nella quale vengono riportate le informazioni riguardanti le scelte effettuate dall'utente e i suoi dati di navigazione. Tramite questa pagina può scegliere nuove immagini oppure cancellare i propri dati dal database.
* images.html: è la pagina del dominio applicativo, in cui l'utente sceglie le opere d'arte che preferisce.
* report.html: è la pagina che permette di consultare le informazioni raccolte sul comportamento degli utenti e sulle loro preferenze.

## Tecnologie utilizzate/implementate
Le tecniche utilizzate/implementate per profilare il singolo utente sono le seguenti:
* Canvas Fingerprint (versione 1 e 2)
* Evercookie
* Tracking Pixel (tramite cookie)
* Cross-Browser Fingerprint

Le tecniche utilizzate/implementate per raccogliere e/o visualizare le informazioni riguardo il comportamento degli utenti sono le seguenti:
* Ad Tracking (tramite metrica click-through rate)
* Geolocalizzazione (tramite libreria geoPlugin e Google Maps API)
* Affluenza dell'utenza (fascia oraria / giorno della settimana)
* Preferenza dell'utenza
* Mouse Tracking
