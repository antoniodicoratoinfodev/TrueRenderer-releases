# Installazione macOS — anteprima

1. Scarica lo ZIP macOS e `SHA256SUMS.txt` dagli allegati della release pubblica; non serve un account GitHub. Gli archivi automatici “Source code” contengono la documentazione, non l'app.
2. Nella cartella dei download verifica `shasum -a 256 -c SHA256SUMS.txt`.
3. Estrai lo ZIP e sposta **l'intera cartella** in una posizione scrivibile, per esempio `~/Applications/TrueRenderer-0.1.5-macos-arm64/`. Conserva app, corpus, avviatore e sorgenti/avvisi di terzi insieme.
4. Avvia **Avvia TrueRenderer.command**. Questo avviatore imposta risorse e dati separati dal progetto di sviluppo. Non spostare la sola `.app` e non usare il doppio clic diretto sull'app per questa anteprima.

Il pacchetto ha firma ad hoc, senza Developer ID o notarizzazione. macOS può impedirne l'apertura dopo il download. Non è un installer pubblico qualificato: se bloccato, contatta il titolare; queste istruzioni non richiedono di disattivare Gatekeeper.

L'avviatore usa `~/Library/Application Support/TrueRenderer-Preview/` per catalogo, preferenze, cache e backup. Non condividere questa directory tra istanze contemporanee. Il pacchetto scrive anche la cartella `reports/` accanto al corpus.

Per aggiornare, chiudi l'app, conserva una copia consistente della directory dati e sostituisci l'intera cartella del pacchetto. Non riaprire un catalogo migrato con un'app precedente senza verificarne la compatibilità. Per rimuovere l'app, elimina la cartella del pacchetto; i dati restano nella directory del profilo e non vanno cancellati come cache.

L'accesso al repository non sostituisce il permesso d'uso previsto dalla [licenza](LICENSE).
