# Initial Network State

**Notre objectif initial n'est pas de trouver un prix stable**. Cela peut sembler contre-intuitif mais Olympus peut être réglé pour optimiser différentes choses. Le principal compromis est la volatilité et la rentabilité par rapport à la stabilité et la durabilité. Avec la volatilité et le profit vient la croissance ; c'est ce que nous voulons dès le début.

Avec une politique monétaire rigoureuse et de la traction, Olympus devrait bien fonctionner comme un actif stable. Les pressions à la hausse et à la baisse devraient se stabiliser à une certaine valeur \(non intrinsèque\). Avec une politique souple, indépendamment de l'échelle, Olympus a le potentiel d'agir comme une machine à créer de la richesse. Le marché primaire du token mesure la balance positive ; toute valeur extrinsèque est une nouvelle richesse créée.

## Alpha State

Le réseau initial comporte une trésorerie à sens unique \(l'argent entre, rien ne sort\), le contrat d'obligation \(par lequel l'offre augmente et les profits sont produits\), et le contrat de staking \(où les profits sont distribués\).

Les états initiaux de la stratégie sont les suivants :

* **BCV**

  La [BCV](https://docs.olympusdao.finance/references/glossary#bcv) varie en fonction des types d'obligations. Elle est régulièrement ajustée par l'équipe qui gère la politique monétaire \(politic team\) pour répondre aux objectifs du protocole. Par exemple, si le protocole veut accumuler plus de liquidités dans sa trésorerie, il peut baisser la BCV des [liquidity bonds](https://docs.olympusdao.finance/references/glossary#liquidity-bonds) pour augmenter leur capacité obligataire. Pour consulter les objectifs de la BCV pour les différents types d'obligations, visitez [Olympus Policy Dune page](https://dune.xyz/shadow/Olympus-Policy).

* **Durée d'acquisition des obligations**

  Il est fixé à 33110 blocs d'Ethereum ou environ cinq jours pour tous les types d'obligations.

* **Distribution des OHM**

  Chaque fois que des obligations sont achetées, le produit de l'opération est versé à la trésorerie [Olympus](https://docs.olympusdao.finance/references/contracts#treasury). Le montant correspondant en OHM sera mint et distribué à 3 parties : 

  * **Bonder**

    L'acheteur de l'obligation recevra le montant cité de l'OHM de façon linéaire sur la période d'acquisition.

  * **DAO**

    La DAO reçoit la même quantité d'OHM que le bonder. Cela représente le bénéfice du DAO

  * **Stakers**

    Après avoir distribués les OHM au bonder et à la DAO, le reste sera distribué entre tous les stakers du protocole.

