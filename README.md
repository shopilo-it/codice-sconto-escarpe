# Codice sconto eScarpe, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto eScarpe** da [shopilo.it](https://shopilo.it/negozi/escarpe.it). Restituisce **coupon eScarpe** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-escarpe](https://shopilo-it.github.io/codice-sconto-escarpe/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-escarpe
cd codice-sconto-escarpe
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "eScarpe",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su calzature",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/escarpe.it"
  }
]
```

## Coupon eScarpe disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su calzature | [shopilo.it](https://shopilo.it/negozi/escarpe.it) |

Codici attivi: **[shopilo.it/negozi/escarpe.it](https://shopilo.it/negozi/escarpe.it)**

## Domande frequenti

### Come utilizzo un codice sconto eScarpe?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/escarpe.it), aggiungi i prodotti al carrello su eScarpe e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon eScarpe?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher eScarpe piu recenti?
La pagina [shopilo.it/negozi/escarpe.it](https://shopilo.it/negozi/escarpe.it) viene aggiornata quotidianamente con i codici sconto eScarpe, voucher eScarpe e coupon promozionali eScarpe piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su eScarpe

eScarpe e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/escarpe.it) trovi i migliori codici sconto eScarpe, coupon eScarpe verificati e voucher eScarpe attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-escarpe
```

```javascript
const { fetchCoupons } = require('codice-sconto-escarpe');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
