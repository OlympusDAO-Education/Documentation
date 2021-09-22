# Acheter une obligation \(1, 1\)

Les obligations permettent aux utilisateurs d'acheter des OHM du protocole à un prix réduit en les échangeant contre divers actifs, les LP token \(appelé [liquidity bonds](https://docs.olympusdao.finance/v/francais/basics/glossary#liquidity-bonds)\) ou du DAI & Frax \([reserve bonds](https://docs.olympusdao.finance/v/francais/basics/glossary#reserve-bonds)\).

Les obligations prennent environ 15 epochs pour être acquises et l'utilisateur acquiert ses $OHM de manière linéaire sur cette même période. Les obligations de liquidité aident le protocole à accumuler et à bloquer des liquidités, tandis que les obligations de réserve permettent au protocole d'accroître sa trésorerie, et donc sa [RFV](https://docs.olympusdao.finance/v/francais/basics/glossary#rfv) plus rapidement.

Il y a 5 type de bonds sur [Olympus](https://app.olympusdao.finance/#/bonds) :

* [DAI bond](bond_dai.md)
* [FRAX bond](bond_frax.md)
* [wETH bond](bond_weth.md)
* [OHM-DAI LP bond](ohm-dai-lp-bond.md)
* [OHM-FRAX LP bond](bond_ohm_frax.md)

## Hades

Hades est une fonctionnalité qui vous permet d'acheter des obligations tout en envoyant les OHM acquises à une autre adresse. Ceci est utile pour plus de confidentialité ou pour acheter plusieurs obligations alors que les obligations actuelles sont encore en cours d'acquisition. Notez que si le même compte détient plusieurs obligations, les récompenses en attente des obligations précédentes doivent être abandonnées. 

1. Allez sur [Bond page](https://app.olympusdao.finance/#/bonds) et sélectionnez le type d'obligation que vous souhaitez acheter.
2. Sélectionnez le montant que vous souhaitez acheter, puis cliquez sur l'icône en forme de roue dentée en haut à droite de la page.

   ![](../../.gitbook/assets/cogwheel.png)

3. Le menu Hades s'affiche. Dans le champ Adresse du destinataire, vous pouvez indiquer une adresse différente qui recevra l'OHM acquis. Par défaut, le champ est rempli avec votre adresse actuelle.

   ![](../../.gitbook/assets/hades.png)

4. Vous pouvez également modifier le champ slippage pour augmenter ou diminuer la probabilité que votre ordre soit exécuté. Un slippage plus élevé augmente cette probabilité, mais vous pouvez obtenir un prix de remplissage plus indésirable. 
5. Fermez le menu Hades en cliquant à nouveau sur l'icône en forme de roue dentée. 
6. Cliquez sur "Approve" et signez la transaction. 
7. Une fois que la transaction "Approve" a été traitée avec succès, cliquez sur "Bond" et signez la transaction. Voilà, vous avez acheté votre première obligation en utilisant Hades !  _NB : La transaction "Approve" n'est nécessaire que lors de première interaction avec le smart contract ; pour les suivantes, il suffit d'effectuer la transaction "Bond". Lorsque vous utilisez Hades, ne modifiez pas le montant du cautionnement après avoir fermé le menu Hades, car cela réinitialiserait l'adresse du destinataire._

## **Comment racheter \(redeem\)**

Allez sur [Bond page](https://app.olympusdao.finance/#/bonds) et sélectionnez le type d'obligation que vous avez acheté. Sélectionnez l'onglet "Redeem". Ensuite, cliquez sur "Claim Rewards" pour réclamer toutes vos récompenses disponibles.

## Infos

![](../../.gitbook/assets/modal.png)

**Balance** est votre solde de tokens SLP. C'est l'actif utilisé pour créer une obligation.   
  
**Bond price** est le prix de l'OHM que vous obtenez en créant une obligation. Vous pouvez calculer le prix de l'obligation en utilisant les formules suivantes : 

* Obligation SLP : \(Valeur de votre token SLP / OHM que vous obtiendrez en créant des obligations\) 
* Obligation DAI : \(Valeur de votre token DAI / MH que vous obtiendrez en cautionnant\) 

**Market Price** est le prix du marché des OHM.   
  
**You Will Get** indique combien de OHM vous obtiendrez en cautionnant. Le ratio d'endettement mesure le montant total de OHM créé à partir des obligations qui doivent encore être payées par le protocole. Le ratio d'endettement est calculé différemment pour le cautionnement SLP et le cautionnement DAI :

* Obligation SLP : \(OHM créé à partir des obligations non remboursées / approvisionnement total en OHM\) 
* Obligation DAI : \(MRO créé à partir d'obligations non remboursées / MRO en circulation\). 

**Vesting term** mesure la période nécessaire au remboursement intégral d'une obligation. Ce nombre est exprimé en blocs d'Ethereum. 33110 blocs correspondent à environ 5 jours ou 15 époques. 

**Discount** est la différence entre le prix de l'obligation et le prix du marché. Dans la capture d'écran ci-dessus, l'obligation vous donnerait un rabais de 10,63% par rapport à l'achat de la même quantité d'OHM sur le marché.

![](../../.gitbook/assets/modal_redeem.png)

L'OHM que vous êtes en droit de recevoir par obligation.

**Claimable Rewards** sont le montant des OHM que vous pouvez réclamer maintenant. Ce montant augmente au fur et à mesure que les OHM vous sont acquis au cours de la période d'obligation.

**Full Bond Maturation** fait référence au bloc d'Ethereum lorsque l'obligation est entièrement remboursable.

