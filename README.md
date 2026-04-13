# Code promo EMP, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo EMP** depuis [shopilo.fr](https://shopilo.fr/reductions/emp-online.fr). Renvoie les **coupons EMP** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-emp](https://shopilo-fr.github.io/code-promo-emp/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-emp
cd code-promo-emp
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "EMP",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur le merchandising et les vetements rock",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/emp-online.fr"
  }
]
```

## Coupons EMP disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur le merchandising et les vetements rock | [shopilo.fr](https://shopilo.fr/reductions/emp-online.fr) |

Codes actifs : **[shopilo.fr/reductions/emp-online.fr](https://shopilo.fr/reductions/emp-online.fr)**

## Questions frequentes

### Comment utiliser un code promo EMP ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/emp-online.fr), ajoutez les produits a votre panier sur EMP et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons EMP ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction EMP les plus recents ?
La page [shopilo.fr/reductions/emp-online.fr](https://shopilo.fr/reductions/emp-online.fr) est mise a jour quotidiennement avec les codes promo EMP, bons de reduction EMP et coupons promotionnels EMP les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de EMP

EMP est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/emp-online.fr), retrouvez les meilleurs codes promo EMP, coupons EMP verifies et bons de reduction EMP actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-emp
```

```javascript
const { fetchCoupons } = require('code-promo-emp');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
