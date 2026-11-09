# Cosa Indosso 👔

App per scegliere ogni giorno **cosa indossare**, in base a meteo, occasione e colori dei capi del tuo armadio.
Funziona interamente sul dispositivo: nessun account, nessun server, nessun dato inviato a terzi (a parte la richiesta del meteo).

## Funzioni

- **Outfit del giorno** calcolato con regole di stile (abbinamento colori, formalità, isolamento termico, pioggia)
- **Armadio digitale** con foto facoltative, colori precisi e stato "in lavaggio"
- **Meteo** a 7 giorni tramite Open-Meteo (solo la città, nessuna registrazione)
- **Occasioni**: casual, smart, elegante, sport
- **Diario** degli outfit indossati, con foto, e outfit salvati
- **Valigia** per viaggi: outfit giorno per giorno usando meno capi possibile
- **Accessori**: borse, orologi e profumi abbinati all'outfit
- **Da comprare**: classifica dei capi che ti aprono più outfit nuovi
- **Capi dimenticati**, analisi dell'armadio, tema chiaro/scuro con colori stagionali
- **Backup e ripristino** in JSON

## Provarla subito

Apri `index.html` in un browser moderno (anche da telefono). I dati restano nel `localStorage` e in IndexedDB del browser.

Versione online (se attivi GitHub Pages): `https://TUO-UTENTE.github.io/NOME-REPO/`

## Struttura

```
index.html                       app completa (HTML + CSS + JS, nessuna dipendenza)
fonts/PlayfairDisplay-Regular.woff2   font dei titoli
LICENSE                          licenza MIT
NOTICE.md                        attribuzioni di terze parti
```

## App Android (opzionale)

L'interfaccia è pensata per essere inserita in un wrapper [Capacitor](https://capacitorjs.com/). Se il wrapper è presente, l'app usa in più:
notifiche locali (outfit del mattino e della sera), backup automatico settimanale in Documenti, condivisione del backup e widget.
Nel browser queste funzioni sono semplicemente disattivate; il resto funziona uguale.

## Privacy

Armadio, diario e foto non lasciano il dispositivo. L'unica chiamata di rete è verso Open-Meteo, che riceve le coordinate della città scelta per restituire le previsioni.

## Crediti

- Dati meteo: [Open-Meteo.com](https://open-meteo.com/) (licenza CC BY 4.0, uso gratuito non commerciale)
- Font: Playfair Display (SIL Open Font License 1.1)

## Licenza

[MIT](LICENSE)
