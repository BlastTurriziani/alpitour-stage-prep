Guida al Deploy – GiMTonic

Questa guida descrive i passaggi eseguiti per pubblicare il progetto GiMTonic su Azure.


1 Creazione risorse Azure

App Service
- Risorsa: gimtonic-web
- Gruppo di risorse: rg-gimtonic-prod
- Runtime: .NET 8 / Linux
- Regione: West Europe
- Piano: Basic (B1)

Storage Account
- Nome: stgimtonicprod
- Tipo: StorageV2 (general purpose)
- Accesso pubblico: abilitato
- Funzionalità usata: Static Website


2 Pubblicazione del sito
- File index.html creato in locale
- Compresso in .zip e caricato nella sezione Deployment Center
- Verificata la presenza del file in /site/wwwroot via SSH
- Test del link pubblico:
  https://gimtonic-web-xxxxxx.westeurope-01.azurewebsites.net


3 Sicurezza e test
- HTTPS forzato
- Controllo accessi con identità gestita (MS Entra ID)
- Monitoraggio con Application Insights (facoltativo)


4 Versionamento su GitHub
- Repository: alpitour-stage-prep
- Path del progetto: /azure/gimtonic
- Commit tipico:
  git add .
  git commit -m "Deploy iniziale progetto GiMTonic su Azure"
  git push origin main


Note finali
Questo progetto rappresenta un didattico 
per la gestione di una palestra digitale, pubblicato con risorse cloud gratuite (Azure for Students).
