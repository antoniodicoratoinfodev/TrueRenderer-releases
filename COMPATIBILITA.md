# Compatibilità e limiti

- Pacchetto disponibile: macOS Apple Silicon (`arm64`), versione app 0.1.5, build 6, snapshot del 2 novembre 2026.
- Verifica del pacchetto eseguita su macOS 27.2. Versione minima del sistema e funzionamento su altri Mac non qualificati; nessun pacchetto Intel/universal.
- Due decoder XPC con App Sandbox; firma ad hoc, nessuna notarizzazione o qualifica per il rilascio pubblico.
- JPEG, PNG e TIFF; RAW dipendenti da modello, motore e versione macOS. Nessuna compatibilità universale.
- Integrata mostra il JPEG fotocamera, fino a 2048 pixel, quando presente in un contenitore riconosciuto. Le modifiche RAW sono conservate ma sospese. Tornare a Piena per sviluppo ed esportazione.
- Il motore indipendente trueRendererExperimental 32fp resta sperimentale. Le etichette di qualità nell'interfaccia non sono una certificazione della resa.
- Windows: pacchetto da aggiungere in una consegna successiva. Nessun download Windows disponibile qui.
