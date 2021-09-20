# Borrowing

Vous pouvez commencer par consulter [l'article Medium ](https://davidgmi.medium.com/how-to-cast-a-magic-spell-to-your-ohm-and-3-3-strategy-using-abracadabra-money-45fc6187f281)de David sur la façon d'utiliser Abracadabra, en plus des explications de base ci-dessous.

## Comment emprunter du MIM

Si vous avez des OHM sur Olympus vous pouvez emprunter du MIM contre votre sOHM.  
  
1. Connectez votre wallet sur [Abracadabra.money Pool 10](https://abracadabra.money/pool/10).  
  
2. Dans le menu "WRAP", wrap le montant de sOHM avec lequel vous souhaitez emprunter, pour du wsOHM. 

![](../../.gitbook/assets/screen-shot-2021-08-29-at-4.10.42-pm%20%281%29.png)

3. Allez dans le menu "BORROW" \(emprunter\). Saisissez le montant de wsOHM que vous voulez utiliser comme garantie puis saisissez le montant de MIM que vous voulez emprunter.   
  
4. Cliquez sur "ADD COLLATERAL AND BORROW" et signez la transaction. Lorsque la transaction est traitée avec succès, le montant de MIM emprunté apparaît dans votre wallet.

{% hint style="info" %}
Si c'est votre première interaction avec l'application, vous devez d'abord approuver le contrat d'Abracadabra pour dépenser vos tokens.
{% endhint %}

{% hint style="warning" %}
Assurez-vous de comprendre le fonctionnement de l'effet de levier dans cet article \(anglais\) [Abracadabra](https://docs.abracadabra.money/intro/leveraged-positions).
{% endhint %}

![](../../.gitbook/assets/screen-shot-2021-08-29-at-4.10.54-pm%20%281%29.png)

1. Cliquez sur "Change leverage" et choisissez un montant de boucle.

2. En fonction du montant de la boucle \(de 1 à 10\), le montant de votre emprunt, l'effet de levier et le prix de liquidation seront mis à jour en conséquence.

{% hint style="danger" %}
Le prix de liquidation augmente avec le montant de la boucle, et un prix de liquidation plus élevé signifie que vous pouvez être liquidé plus facilement.
{% endhint %}

3. Vous pouvez ajuster la "Swap Tolerance". Une valeur plus faible signifie que votre transaction est plus susceptible d'échouer, par exemple lorsque le taux du MIM change pendant l'exécution de votre transaction.

4. Pour utiliser un prix de gaz inférieur, cliquez sur "Update price". Cliquez ensuite sur "ADD COLLATERAL AND BORROW" et signez la transaction pour ouvrir une position à effet de levier.

5. Contrairement à un emprunt normal, vous n'obtiendrez pas de jetons MIM dans votre portefeuille à la suite de cette transaction, car ils sont échangés contre plus de wsOHM \(en arrière-plan\).

{% hint style="danger" %}
Vous pouvez ajouter des garanties supplémentaires \(collateral\) avant que dépôt n'atteigne le prix de liquidation. Lorsque vous utilisez l'effet de levier, vous perdez tout vos collateral si vous êtes liquidé.
{% endhint %}

