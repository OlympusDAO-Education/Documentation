# La migration v2

## Pourquoi migrons nous ? <a href="#why-do-i-need-to-migrate" id="why-do-i-need-to-migrate"></a>

La migration V2 introduit de nouvelles fonctionnalités telles que la gouvernance on-chain et l'auto-stake pour les obligations. La transition de sOHM V1 à gOHM permet de prendre plusieurs obligations à la fois, par opposition à une obligation par période d'acquisition comme c'était le cas dans v1. Une liquidité partielle restera pour v1 OHM pendant la migration. Cela permet aux emprunteurs de disposer de liquidités suffisantes pour clôturer ou déplacer leur position d'emprunt. Vous pouvez en savoir plus à ce sujet sur la page [Olympus Medium page](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

{% hint style="info" %}
**Vous avez deux mois pour migrer** après le lancement de la V2. Si vous ne le faites pas, votre solde sOHM V1 cessera de rebase, **mais la différence sera honorée lorsque vous migrez.** &#x20;
{% endhint %}

{% hint style="info" %}
Pour cet article, nous avons ajouté V1 et V2 après chaque nom de token pour vous aider à différencier les anciens et les nouveaux tokens. Les sites Web des partenaires, les agrégateurs de prix ou votre portefeuille n'afficheront pas les informations relatives à la version.
{% endhint %}

## Quel est le TLDR? <a href="#what-is-the-tldr" id="what-is-the-tldr"></a>

* wsOHM V1 (wrapped, staked OHM) sera remplacé par gOHM (Governance OHM). Leurs fonctions sont similaires, mais gOHM est requis pour la gouvernance on-chain.
* OHM & sOHM auront également leur v2. OHM V1 devient OHM V2, et sOHM V1 devient sOHM V2.
* Les tickers des jetons resteront les mêmes pour les jetons V1. Par exemple, après la migration, votre portefeuille affichera "OHM" au lieu de "OHM V1". Veillez à mettre à jour le contrat de tokens dans votre portefeuille avec [V2 addresses](https://app.gitbook.com/o/-MYfkWbCEr4-AnVvIx6p/s/-MV4hwONledQK5nEDaUc-887967055/contracts/tokens) pour afficher votre solde.
* Lors de la migration de OHM V1 et/ou sOHM V1, vous obtiendrez des gOHM en retour. Bien que le solde de jetons soit différent (le prix du gOHM est calculé différemment, en fonction de l'indice actuel), **le montant en dollars reste le même.**
* Après la migration, les pools OHM V1 tels que OHM-DAI utiliseront OHM V2. Ceci s'applique également aux nouveaux dépôts. Les partenaires comme Abracadabra n'accepteront les nouveaux dépôts en gOHM uniquement. Vous devrez donc migrer si vous voulez utiliser ces fonctionnalités. Sinon, vous pouvez rester tranquille et ne migrer que lorsque vous le souhaitez.

## Et si ne je migre pas ? <a href="#what-if-i-dont-migrate" id="what-if-i-dont-migrate"></a>

Vous ne pourrez pas profiter des nouvelles fonctionnalités introduites par la V2. Certains partenaires, comme Rari Capital, n'accepteront les tokens V2 qu'une fois qu'ils seront déployés. Vous devrez donc migrer si vous souhaitez utiliser plus de tokens (par exemple, effectuer de nouveaux dépôts) sur ces plateformes.

## Les Gas fees sont élevées maintenant, vais-je perdre mes récompenses de rebase si je retarde la migration ? <a href="#gas-fees-are-high-now-will-i-lose-my-rebase-rewards-if-i-delay-the-migration" id="gas-fees-are-high-now-will-i-lose-my-rebase-rewards-if-i-delay-the-migration"></a>

Non, vous pourrez migrer à votre guise dès que le système sera opérationnel. Le contrat intelligent gardera la trace de vos récompenses de rebasement autorisées afin que vous n'en manquiez aucune.

## Quel est le processus de la migration ? <a href="#what-is-the-migration-process" id="what-is-the-migration-process"></a>

Lorsque la migration sera effective, le front-end d'Olympus sera mis à jour pour permettre la migration de tous vos tokens V1 (c.-à-d. OHM, sOHM et wsOHM) vers le serveur d'Olympus. Le processus de migration nécessite deux étapes : une pour approuver le contrat pour chacun de vos tokens V1, et une autre qui migre effectivement tous vos tokens vers le serveur d'Olympus. Par exemple, si vous avez OHM V1 et sOHM V1 dans votre portefeuille, vous devez effectuer deux approbations de jetons, mais une seule opération de migration (trois transactions au totale).

## Puis-je migrer un type spécifique de token V1 et laisser les autres de côté ? <a href="#can-i-migrate-a-specific-type-of-v1-token-and-leave-out-the-others" id="can-i-migrate-a-specific-type-of-v1-token-and-leave-out-the-others"></a>

Non. Vous pouvez soit migrer tous vos tokens V1 (c'est-à-dire OHM, sOHM et wsOHM), soit aucun.

## Puis-je revenir après la migration v1 en gOHM? <a href="#can-i-switch-back-to-v1-tokens-after-migrating-them-to-gohm" id="can-i-switch-back-to-v1-tokens-after-migrating-them-to-gohm"></a>

Non, vous ne pouvez revenir en arrière après avoir la migration.

## Pouvez-vous me donner un exemple de ce que je peux attendre de la migration ? <a href="#can-you-walk-me-through-an-example-of-how-much-gohm-i-can-expect-from-the-migration" id="can-you-walk-me-through-an-example-of-how-much-gohm-i-can-expect-from-the-migration"></a>

Supposons que vous ayez 20 OHM V1, 20 sOHM V1, et 20 wsOHM, et que le [Current Index](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards) soit de 10.&#x20;

* 20 OHM V1 = 2 gOHM. Prenez vos 20 OHM et divisez-les par le [Current Index](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards) pour obtenir vos gOHM.
* 20 sOHM V1 = 2 gOHM. Prenez vos 20 sOHM et divisez-les par le [Current Index](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards) pour obtenir vos gOHM.
* 20 wsOHM = 20 gOHM. 1 wsOHM = 1 gOHM.

Pour rappel, si vous migrez d'un token non indexé (OHM, sOHM) vers un token indexé (gOHM), vous ne recevrez pas la même quantité de tokens après la migration, **mais ils ont toujours la même valeur en dollars.**

## Est-ce que mon gOHM continuera à recevoir lees rebase rewards? <a href="#will-my-gohm-still-earn-rebase-rewards" id="will-my-gohm-still-earn-rebase-rewards"></a>

Oui. Bien que la quantité de gOHM ne change pas lors d'un rebasement comme c'est le cas pour la sOHM, elle vous permet de gagner des récompenses de rebasement. En effet, le prix du gOHM est lié à l'indice actuel :

$$
gOHM_{price} = OHM_{price} * CurrentIndexgOHMprice
$$

Chaque rebase entraîne une augmentation du Current Index, et votre gOHM a donc plus de valeur (à condition que le prix de l'OHM reste constant).

## Comment les obligations sont-elles affectées après la migration? <a href="#how-are-bonds-affected-after-the-migration" id="how-are-bonds-affected-after-the-migration"></a>

Dans la V2, vous pouvez acheter plusieurs obligations du même type sans réinitialiser la période d'acquisition des obligations. De même, il n'est pas nécessaire de réclamer des récompenses en obligations et de les mettre en jeu manuellement, car ce processus sera automatisé. Les détenteurs d'obligations recevront leurs sOHM à la fin de la période d'acquisition. Pour en savoir plus sur le comportement des obligations dans la V2, consultez [Olympus Medium page](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

## Olympus V2 est audité? <a href="#is-olympus-v2-audited" id="is-olympus-v2-audited"></a>

Tous les contrats liés à la V2 sont en ligne, et certains d'entre eux sont encore en cours d'audit. Nous travaillons avec Runtime Verification pour l'audit, et les résultats seront publiés dès qu'ils seront disponibles.
