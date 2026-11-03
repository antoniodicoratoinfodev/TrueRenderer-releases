# Installazione — anteprime

## macOS Apple Silicon

1. Scarica lo ZIP macOS e `SHA256SUMS.txt` dagli allegati della release pubblica; non serve un account GitHub. Gli archivi automatici “Source code” contengono la documentazione, non l'app.
2. Nella cartella dei download verifica `shasum -a 256 -c SHA256SUMS.txt`.
3. Estrai lo ZIP e sposta **l'intera cartella** in una posizione scrivibile, per esempio `~/Applications/TrueRenderer-0.1.5-macos-arm64/`. Conserva app, corpus, avviatore e sorgenti/avvisi di terzi insieme.
4. Avvia **Avvia TrueRenderer.command**. Questo avviatore imposta risorse e dati separati dal progetto di sviluppo. Non spostare la sola `.app` e non usare il doppio clic diretto sull'app per questa anteprima.

Il pacchetto ha firma ad hoc, senza Developer ID o notarizzazione. macOS può impedirne l'apertura dopo il download. Non è un installer pubblico qualificato: se bloccato, contatta il titolare; queste istruzioni non richiedono di disattivare Gatekeeper.

L'avviatore usa `~/Library/Application Support/TrueRenderer-Preview/` per catalogo, preferenze, cache e backup. Non condividere questa directory tra istanze contemporanee. Il pacchetto scrive anche la cartella `reports/` accanto al corpus.

Per aggiornare, chiudi l'app, conserva una copia consistente della directory dati e sostituisci l'intera cartella del pacchetto. Non riaprire un catalogo migrato con un'app precedente senza verificarne la compatibilità. Per rimuovere l'app, elimina la cartella del pacchetto; i dati restano nella directory del profilo e non vanno cancellati come cache.

L'accesso al repository non sostituisce il permesso d'uso previsto dalla [licenza](LICENSE).

## Windows x64

1. Scarica **TrueRenderer-0.1.6-Setup-x64.exe** e il relativo file `.sha256` dalla release Windows pubblica; non serve un account GitHub. Gli archivi automatici “Source code” contengono la documentazione, non l'app.
2. Nella cartella dei download esegui in PowerShell `Get-FileHash .\TrueRenderer-0.1.6-Setup-x64.exe -Algorithm SHA256` e confronta il valore con quello nel file `.sha256`.
3. Chiudi TrueRenderer se aperto, avvia l'installer e segui la procedura. L'installazione è per il tuo utente, senza privilegi amministrativi, in `%LOCALAPPDATA%\Programs\TrueRenderer`. Il collegamento Desktop e l'associazione dei file `.truerenderer` sono opzioni dell'installer.
4. Avvia TrueRenderer dal menu Start o dal collegamento creato.

Richiede Windows 10/11 x64 e dispositivo/driver grafico compatibile. ARM64 non qualificato. Installer, app e worker non sono firmati: SmartScreen o Smart App Control possono impedirne l'esecuzione. Non è richiesto di disattivare le protezioni di Windows.

Per aggiornare, chiudi l'app, conserva un backup consistente dei dati ed esegui il nuovo installer. Catalogo, preferenze, cache e backup restano separati dai programmi in `%LOCALAPPDATA%\TrueRenderer\var`. Questi dati rimangono anche dopo la disinstallazione e non vanno cancellati come cache. Gli originali fotografici restano in sola lettura.

Il pacchetto include worker isolato LPAC, runtime grafico DXC, corpus sintetico, licenze, avvisi e sorgenti coperti delle dipendenze. Non richiede Rust, Visual Studio o la toolchain di sviluppo.
