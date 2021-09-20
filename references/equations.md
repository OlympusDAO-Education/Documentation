# Equations

## Staking

$$
deposit = withdrawal
$$

Les échanges entre OHM et sOHM pendant le staking et l'unstaking sont toujours honorés 1 pour 1. La quantité d'OHM déposée dans le contrat de staking donnera toujours lieu à la même quantité de sOHM. Et la quantité de sOHM retirée du contrat de staking donnera toujours lieu à la même quantité de OHM.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

Le trésorerie dépose les OHM dans le distributeur. Le distributeur dépose ensuite des OHM dans le contrat de staking, ce qui crée un déséquilibre entre les OHM et les sOHM. Les sOHM sont rebasés pour corriger ce déséquilibre entre les OHM déposés et les sOHM en circulation. Le rebase ramène les sOHM en circulation à la parité, de sorte que 1 sOHM est égal à 1 OHM stake.

## Bonding

$$
bond Price = 1 + Premium
$$

L'OHM a une valeur intrinsèque de 1 DAI, ce qui équivaut approximativement à 1 $. Afin de réaliser un profit sur les obligations, Olympus demande un premium pour chaque obligation.

$$
Premium = debt Ratio * BCV
$$

Le premium est dérivé du ratio d'endettement du système et d'une variable d'échelle appelée [BCV](https://docs.olympusdao.finance/references/glossary#bcv). La BCV nous permet de contrôler le taux d'augmentation du prix des obligations.

Le premium détermine le profit dû au protocole et, à son tour, aux stakers. En effet, de nouveaux OHM sont frappés à partir du bénéfice et ensuite distribués à tous les stakers.

$$
debt Ratio = bondsOutstanding/ohmSupply
$$

Le ratio d'endettement est le total de tous les OHM promis aux obligataires divisé par l'offre totale d'OHM. Cela nous permet de mesurer la dette du système.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

Le paiement de l'obligation détermine le nombre d'OHM vendus à un obligataire. Pour les [reserve bonds](https://docs.olympusdao.finance/references/glossary#reserve-bonds), la valeur marchande des actifs fournis par le bonder est utilisée pour déterminer le paiement de l'obligation. Par exemple, si un utilisateur fournit 1000 DAI et que le prix du cautionnement est de 250 DAI, l'utilisateur aura droit à 4 OHM.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

Pour [les liquidity bonds](https://app.gitbook.com/@0xmule/s/olympus-dao/~/drafts/-MiRtBb2Fh1mGoE5J5Ud/referre-ce/lexique/@merged#liquidity-bonds), la valeur marchande des jetons LP fournis par l'émetteur est utilisée pour déterminer le paiement de l'obligation. Par exemple, si un utilisateur fournit 0,001 jeton LP OHM-DAI dont la valeur est de 1000 DAI au moment de l'obligation, et que le prix de l'obligation est de 250 DAI, l'utilisateur aura droit à 4 OHM.

## OHM Supply

$$
OHM_{supplyGrowth} = OHM_{stakers} + OHM_{bonders} + OHM_{DAO}
$$



La réserve totale d'OHM n'a pas de plafond fixe. Son offre augmente quand : 

* Les OHM sont mint et distribués aux stakers.
* Les OHM sont mint pour le bonder et la DAO lorsque quelqu'un achète une obligation. La DAO reçoit le même nombre de OHM que le bonder.

$$
OHM_{stakers} = OHM_{totalSupply} * rewardRate
$$

A la fin de chaque epoch, la trésorerie frappe des OHM à [reward rate](https://docs.olympusdao.finance/references/glossary#reward-rate) fixé. Ces OHM seront distribués à tous les stakers du protocole. Vous pouvez suivre le dernier taux de récompense sur le [Olympus Policy dashboard](https://dune.xyz/shadow/Olympus-Policy).

$$
OHM_{bonders} = bondPayout
$$

Chaque fois qu'une personne achète un bond, un nombre déterminé d'OHM est frappé. Ces OHM ne seront pas remis au porteur en une seule fois - ils lui sont distribué linéairement au fil du temps. Le paiement des obligations utilise une formule différente pour les différents types d'obligations. Consultez la section [bonding ](equations.md#bonding)ci-dessus pour voir comment il est calculé.

$$
OHM_{DAO} = OHM_{bonders}
$$

La DAO reçoit la même quantité d'OHM que le bonder. Cela représente le bénéfice du DAO.

## Backing per OHM

$$
OHM_{backing} = treasuryBalance_{stablecoin} + treasuryBalance_{otherAssets}
$$

Chaque OHM en circulation est soutenu par la trésorerie d'Olympus. Les actifs de la trésorerie peuvent être divisés en deux catégories : stablecoin et non-stablecoin.

$$
treasuryBalance_{stablecoin} = RFV_{reserveBond} + RFV_{lpBond}
$$

Le solde en stablecoin de la trésorerie augmente lorsque les obligations sont vendues. La [RFV](https://docs.olympusdao.finance/references/glossary#rfv) est calculée différemment pour les différents types d'obligations.

$$
RFV_{reserveBond} = assetSupplied
$$

Pour les reserve bonds telles que l'obligation DAI et l'obligation FRAX, la RFV est simplement égale au montant de l'actif sous-jacent fourni par l'émetteur.

$$
RFV_{lpBond} = 2sqrt(constantProduct) * (\%\ ownership\ of\ the\ pool)
$$

Pour les obligations LP telles que l'obligation OHM-DAI et l'obligation OHM-FRAX, la RFV est calculée différemment car le protocole doit en déprécier la valeur. Pourquoi ? La paire de jetons LP est constituée de OHM, et chaque OHM en circulation sera garantie par ces jetons LP - il existe une dépendance cyclique. Pour assurer que tous les OHM en circulation sont garanties, le protocole dévalue la valeur de ces tokens LP, d'où le nom de valeur sans risque \(RFS\).

