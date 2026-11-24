# Fides Immobiliare — Web Platform (Case Study)

> Il codice sorgente è privato (progetto commissionato). Questo repository descrive in forma pubblica il lavoro svolto.

Piattaforma web full-stack per un'agenzia immobiliare: vetrina pubblica degli annunci, gestione delle richieste dei clienti, area riservata di amministrazione e analytics interno.

## Il mio ruolo
Progettazione e sviluppo end-to-end: architettura, frontend, backend, database, test, CI/CD e messa in produzione.

## Stack
- **Frontend:** React, TypeScript, Vite, React Router
- **Backend:** Node.js, Express, TypeScript
- **Database:** relazionale (MySQL)
- **Test:** Jest, Testing Library
- **Infrastruttura:** VPS Linux, reverse proxy Nginx, process manager PM2, deploy automatizzato con GitHub Actions

## Architettura
- SPA con routing client-side, lazy loading delle immagini e bundle ottimizzato per la produzione.
- API REST con separazione a livelli: **routes → controllers → DAO → modelli/DTO**.
- Middleware dedicati per validazione input, gestione errori, logging e sicurezza.
- Autenticazione dell'area admin basata su token firmati.
- Gestione upload e ottimizzazione immagini tramite servizio esterno.

## Funzionalità
- Catalogo immobili con scheda di dettaglio e filtri
- Modulo di richiesta informazioni e gestione delle richieste
- Dashboard admin per inserire e modificare annunci
- Analytics interno: visite, sessioni, immobili più visti, export in Excel
- Conformità GDPR (cookie banner)

## Qualità e sicurezza (principi adottati)
Validazione e sanitizzazione degli input, rate limiting, header HTTP di sicurezza, gestione dei segreti tramite variabili d'ambiente, nessuna esposizione di dati sensibili al client.

## Sviluppi futuri
- Ricerca avanzata e mappa interattiva
- Notifiche automatiche sulle nuove richieste
- Area clienti con immobili preferiti
- Ottimizzazioni SEO e prestazioni
- Maggiore copertura di test automatici
