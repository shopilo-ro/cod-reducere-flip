# Cod reducere Flip — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Flip** de pe [shopilo.ro](https://shopilo.ro/magazin/flip.ro). Returneaza **cupoane Flip** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-flip](https://shopilo-ro.github.io/cod-reducere-flip/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-flip
cd cod-reducere-flip
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Flip",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la electronice reconditionate",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/flip.ro"
  }
]
```

## Cupoane Flip disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la electronice reconditionate | [shopilo.ro](https://shopilo.ro/magazin/flip.ro) |

Codurile active: **[shopilo.ro/magazin/flip.ro](https://shopilo.ro/magazin/flip.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Flip?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/flip.ro), adauga produsele in cos pe Flip, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Flip?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Flip?
Pagina [shopilo.ro/magazin/flip.ro](https://shopilo.ro/magazin/flip.ro) este actualizata zilnic cu cele mai noi cod reducere Flip, voucher Flip si cupon promotional Flip.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Flip

Flip este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/flip.ro) cele mai bune cod reducere Flip, cupoane Flip verificate si voucher Flip active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-flip
```

```javascript
const { fetchCoupons } = require('cod-reducere-flip');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
