# Fuse

Fuse est un marché de taux d'intérêt de Rari Capital. Chaque pool de Fuse peut supporter différents types d'actifs et utiliser différentes courbes de taux d'intérêt. Pour prêter le sOHM et/ou l'utiliser comme garantie, les utilisateurs peuvent entrer dans le pool [Olympus Pool Party Fuse](https://app.rari.capital/fuse/pool/18). \
\
Dans ce pool, plusieurs actifs sont pris en charge :

* sOHM
* USDC
* DAI
* ETH
* FRAX

## Comment déposer des actifs

1\. Aller sur [Olympus Pool Party Fuse pool](https://app.rari.capital/fuse/pool/18).\
\
2\. Dans le volet _Supply_, sélectionnez l'actif que vous souhaitez déposer. &#x20;

![The Supply panel](../../.gitbook/assets/supply.png)

3\. Saisissez le montant de l'actif que vous souhaitez fournir. Si vous voulez utiliser l'actif comme garantie afin d'emprunter d'autres actifs contre lui, activez le champ "_Collateral_".\
![Enable as collateral](../../.gitbook/assets/collateral.png)

4\. Cliquez sur "_Confirm_". Si c'est la première fois que vous interagissez avec le smart contract, vous devez approuver le contrat pour dépenser votre bien.\
\
5\. Une fois la transaction approuvée vous devez signer une deuxième transaction pour mint le fsToken. fsToken représente votre part dans la pool et vous permet de racheter vos actifs lorsque vous souhaitez les retirer ultérieurement.\
\
6\. Une fois vos fsToken mint, votre actif sera déposé dans la pool Fuse. Cela vous permet de gagner des intérêts et également d'emprunter d'autres actifs si vous avez cochez le champ "_Collateral_".\
\
_Remarque : si vous souhaitez emprunter d'autres actifs contre votre garantie, il y a un montant minimum d'emprunt de 1 ETH en valeur équivalente afin de garantir qu'une liquidation est toujours rentable_\
_(frais de gaz > compte à liquider)_
