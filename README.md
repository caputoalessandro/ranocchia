# Ranocchia

Una piccola sfida al giorno per uscire dalla zona di comfort, con Ranocchia, una rana che cresce con te.
In inglese (predefinito) e in italiano: la lingua si cambia in Settings → Language.
Funziona nel browser, si installa sulla schermata Home e funziona anche offline. Le sfide e le note restano solo sul telefono.

## Contenuto

| File | A cosa serve |
|---|---|
| `index.html` | L'app intera: 162 sfide in inglese e italiano, schermate, mascotte, grafica |
| `manifest.webmanifest` | Nome, colori e icona per l'installazione |
| `sw.js` | Funzionamento offline |
| `icon-*.png` | Icone con la mascotte |
| `.nojekyll` | Dice a GitHub Pages di servire i file così come sono |

## Pubblicare un aggiornamento

1. Sostituisci `index.html` (e gli altri file cambiati) con la nuova versione: Add file → Upload files → Commit.
2. In `sw.js` cambia `VERSION` (per esempio da `ranocchia-v4` a `ranocchia-v5`), così i telefoni scaricano la versione nuova.
3. GitHub Pages aggiorna il sito in un paio di minuti: riapri l'app con la connessione attiva.

I dati restano salvati nel browser di ogni dispositivo e non vengono toccati dagli aggiornamenti.
Per sicurezza, ogni tanto usa Impostazioni → «Esporta in JSON».

## Installare l'app

- Android: apri il sito in Chrome → menu ⋮ → "Installa app".
- iPhone: apri il sito in Safari → Condividi → "Aggiungi alla schermata Home".

## Promemoria

Un'app web non può programmare notifiche quando è chiusa. In Impostazioni → Promemoria, «Aggiungi al calendario»
scarica un evento giornaliero all'orario scelto: aprilo e il calendario del telefono farà da promemoria.
