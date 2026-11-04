# Compatibilità e limiti

- Pacchetto disponibile: macOS Apple Silicon (`arm64`), versione app 0.1.7, build 7, snapshot del 4 novembre 2026.
- Verifica del pacchetto eseguita su macOS 27.2. Versione minima del sistema e funzionamento su altri Mac non qualificati; nessun pacchetto Intel/universal.
- Due decoder XPC con App Sandbox; firma ad hoc, nessuna notarizzazione o qualifica per il rilascio pubblico.
- JPEG, PNG e TIFF; RAW dipendenti da modello, motore e versione macOS. Nessuna compatibilità universale.
- Nel pacchetto macOS 0.1.7, Integrata usa il JPEG fotocamera, fino a 2048 pixel, quando presente in un contenitore riconosciuto. Disponibili regolazioni RGB, ritaglio, prova colore ed export raster da questa rappresentazione; WB sensore conservato ma sospeso. DNG escluso da questo percorso. Le foto visibili e vicine hanno precedenza, poi il resto della cartella viene preparato in sottofondo; l’apertura fredda è progressiva. Il riavvio riprende cartella, foto e qualità salvate; il riuso delle anteprime richiede cache compatibile e conservata entro quota.
- Il motore indipendente trueRendererExperimental 32fp resta sperimentale. Le etichette di qualità nell'interfaccia non sono una certificazione della resa.
- Windows: installer per utente x64, versione 0.1.6, snapshot del 3 novembre 2026. Richiede Windows 10/11 x64 e dispositivo/driver grafico compatibile; ARM64 non qualificato.
- Installer e binari Windows non firmati; SmartScreen o Smart App Control possono bloccarli. Nessuna qualifica su macchine pulite o garanzia di compatibilità universale.
- Decoder Windows eseguito in worker LPAC con limiti Job Object. RAW dipendenti da contenitore, modello e motore selezionato.
- Su Windows Integrata estrae il JPEG dei contenitori TIFF/RAF riconosciuti, fino a 2048 pixel. Disponibili regolazioni RGB, ritaglio, prova colore ed export raster sulla resa della fotocamera; WB sensore sospeso. DNG sensore/lineare richiedono sviluppo RAW. Le foto visibili e vicine vengono preparate su richiesta; l'apertura fredda è progressiva.
