# Codice sconto PrezzoForte, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto PrezzoForte** da [shopilo.it](https://shopilo.it/negozi/prezzoforte.it). Restituisce **coupon PrezzoForte** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-prezzoforte](https://shopilo-it.github.io/codice-sconto-prezzoforte/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-prezzoforte
cd codice-sconto-prezzoforte
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "PrezzoForte",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su outlet elettronica",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/prezzoforte.it"
  }
]
```

## Coupon PrezzoForte disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su outlet elettronica | [shopilo.it](https://shopilo.it/negozi/prezzoforte.it) |

Codici attivi: **[shopilo.it/negozi/prezzoforte.it](https://shopilo.it/negozi/prezzoforte.it)**

## Domande frequenti

### Come utilizzo un codice sconto PrezzoForte?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/prezzoforte.it), aggiungi i prodotti al carrello su PrezzoForte e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon PrezzoForte?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher PrezzoForte piu recenti?
La pagina [shopilo.it/negozi/prezzoforte.it](https://shopilo.it/negozi/prezzoforte.it) viene aggiornata quotidianamente con i codici sconto PrezzoForte, voucher PrezzoForte e coupon promozionali PrezzoForte piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su PrezzoForte

PrezzoForte e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/prezzoforte.it) trovi i migliori codici sconto PrezzoForte, coupon PrezzoForte verificati e voucher PrezzoForte attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-prezzoforte
```

```javascript
const { fetchCoupons } = require('codice-sconto-prezzoforte');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
