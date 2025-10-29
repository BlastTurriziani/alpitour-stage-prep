Documentazione Tecnico-Funzionale – GiMTonic

Obiettivo
Realizzare un prototipo di applicazione web cloud per la gestione di corsi e prenotazioni in palestra, ospitata su Azure App Service.


Attori principali
Ruolo | Descrizione

Cliente | Prenota corsi e gestisce abbonamenti
Istruttore | Gestisce presenze e corsi
Amministratore | Supervisiona utenti e report


Funzionalità chiave
- Login e registrazione utente
- Calendario corsi e disponibilità
- Prenotazione e cancellazione
- Gestione abbonamenti e notifiche


Architettura Azure
[Browser]
   
[Azure App Service] → [Azure SQL Database]

[Azure Storage (Static Website)]


Sicurezza
- HTTPS obbligatorio
- Accesso controllato via Azure AD
- Backup automatici del database
- Key Vault per credenziali


Costi stimati (Azure for Students)
Servizio | Tipo | Costo mensile

App Service | B1 | Gratis / 10 €
Storage | Static Website | Gratis
Database | Basic | 5 €
Totale |   | 15 €/mese (coperto da credito studenti)


Timeline MVP
Settimana | Attività

1-2 | Analisi funzionale
3-4 | Configurazione Azure
5 | Creazione sito statico
6 | Documentazione finale


Autore
Antonio Turriziani  
ITS ICT Piemonte – Cloud Specialist 2025  
Progetto dimostrativo realizzato a scopo formativo.
