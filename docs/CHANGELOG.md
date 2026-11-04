# Changelog

## v0.1.8-macos.20261104

TrueRenderer 0.1.8 per macOS Apple Silicon.

- Nuova icona TR nel bundle macOS e nella finestra dell’app.
- Numero versione allineato a Windows 0.1.8.
- Include ripristino di cartella, foto, vista e qualità per foto, e persistenza delle anteprime della precedente consegna Mac.

Versione sperimentale; i livelli Standard/Piena restano Anteprima. Firma ad hoc, senza notarizzazione; minimo OS e altri Mac non qualificati.

macOS Apple Silicon preview; ad-hoc signed, not notarized. Extract the full folder and use Avvia TrueRenderer.command.

## v0.1.8-windows.20261104

Nuova icona TR per app, barra delle applicazioni, collegamenti e installer Windows. Inclusa la ripresa di cartella, foto, vista e qualit? e il completamento delle scritture anteprime alla chiusura introdotti nei sorgenti 0.1.7. Installer non firmato, limiti di compatibilit? e qualifica invariati. Il download macOS resta 0.1.7; la nuova icona Mac richiede una successiva build verificata su Mac.

## v0.1.7-macos.20261104

TrueRenderer 0.1.7 per macOS Apple Silicon

Riprende l’ultima cartella, la foto selezionata e la vista Anteprima/Griglia all’avvio. Conserva le scelte di qualità per singola foto tra sessioni e cartelle; il cambio globale continua ad azzerarle.

La chiusura normale attende le scritture delle anteprime accettate. Embedded dà precedenza alle foto visibili e ai vicini, poi prepara il resto della cartella in sottofondo. Le anteprime già conservate vengono riusate alla riapertura, nei limiti della cache; lettura, verifica e presentazione richiedono comunque tempo.

Prerelease arm64 con firma ad hoc, non notarizzata. Qualificata su questo Mac; minimi OS e altri Mac non ancora qualificati. Windows resta alla 0.1.6.

macOS Apple Silicon preview; ad-hoc signed, not notarized. Extract the full folder and use Avvia TrueRenderer.command.

## v0.1.6-macos.20261104

TrueRenderer 0.1.6 for macOS Apple Silicon, aligned with the Windows 0.1.6 source version.

- Embedded RAW previews support RGB adjustments, cropping and color proofing, with the same editing recipe retained across preview modes. Sensor white balance stays suspended on the camera JPEG.
- Embedded previews load visible images and nearby photographs on demand.
- Improved editing continuity during rapid adjustments with color proofing, plus faster histogram and JPEG color conversion.
- Raster export from the embedded preview uses that representation, up to 2048 pixels; DNG export is excluded from this path.

Experimental preview. Camera support depends on the selected RAW engine and available embedded JPEG. Matching version numbers do not imply identical platform performance or universal camera support.

macOS Apple Silicon preview; ad-hoc signed, not notarized. Extract the full folder and use Avvia TrueRenderer.command.

## v0.1.6-windows.20261103

Versione Windows allineata a **0.1.6**, compresi app, worker e installer. Funzionalità e limiti dell’anteprima Windows precedente invariati. Checksum e manifest aggiornati; il download macOS resta alla versione 0.1.5.

## v0.1.5-windows.20261103

Prima anteprima Windows x64 con installer per utente, runtime grafico e materiali delle dipendenze inclusi.

- Anteprima Integrata del JPEG fotocamera, con regolazioni RGB, ritaglio, prova colore ed export raster fino a 2048 pixel.
- Preparazione su richiesta delle foto visibili e vicine, con decode JPEG ridotto e caricamento progressivo.
- Continuità dell'editing rapido e della prova colore migliorata.

Installer, app e worker non firmati; SmartScreen o Smart App Control possono bloccarli. Vedi [installazione Windows](INSTALLAZIONE.md#windows-x64) e [compatibilità](COMPATIBILITA.md).

## v0.1.5-macos.20261102

Download resi pubblici e istruzioni aggiornate; binari dell’app invariati.

- Vista Integrata del JPEG incorporato nei RAW, con ritorno esplicito allo sviluppo Piena.
- Pannelli fotografici e raster, livelli, ritocco e prova colore RGB/CMYK.
- Area più ampia per la lista degli strumenti Ritocco.
- Pacchetto portabile con avviatore, fotografie dimostrative pubbliche e materiali delle dipendenze.

La nuova confezione rimuove percorsi locali di compilazione e metadati tecnici interni. Versione per Apple Silicon, con firma ad hoc e senza notarizzazione. Windows sarà aggiunto successivamente.

Vedi [compatibilità](COMPATIBILITA.md) e [installazione](INSTALLAZIONE.md).
