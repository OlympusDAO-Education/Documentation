# Stake ses OHM \(3, 3\)

Parfois, le site Web d'Olympus peut ne pas être accessible en raison de [problèmes d'hébergement](https://twitter.com/FleekHQ/status/1416505712222609411). N'ayez crainte, vous pouvez toujours interagir avec les contrats Olympus pour effectuer certaines actions comme le staking. Dans ce guide, nous allons vous montrer comment stake les OHM via [Etherscan](https://etherscan.io/).

Si vous n'avez jamais stake de OHM auparavant, il y a deux étapes à suivre :

1. Approuver le contrat de staking pour dépenser vos OHM.
2. Stake vos OHM.

Si vous avez déjà stake des OHM, il n'y aura pas à approuver le contrat.

## Comment approuver la dépense du OHM via Etherscan

1. Aller sur dans la section [Write Contract ](https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899#writeContract)du contre OHM.  
  
2. Vérifiez et assurez-vous que le réseau sélectionné est "Ethereum Mainnet" dans votre portefeuille. Appuyez ensuite sur Connect to Web3 pour connecter votre portefeuille si vous ne l'avez pas encore fait.  
  
3. Une fois qu'il est connecté, sélectionnez la troisième option "approve".  
  
4. Dans le champ "_spender \(adresse\)_", nous indiquons l'adresse du contrat de staking.   
Saisissez : **0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d**

5. Dans le champ _\_amount \(uint256\)_, indiquez le montant des OHM que vous souhaitez que le contrat de staking dépense en votre nom, puis multipliez-le par 1e9. Si vous ne voulez pas répéter cette étape à chaque fois que vous voulez miser, vous pouvez choisir une valeur très élevée. Disons que vous voulez permettre au contrat de dépenser jusqu'à 1e9 OHM en votre nom, vous devez entrer : **1'000'000'000'000'000'000**  
  
6. Cliquer sur **Write**  
  
7. Signer la transaction sur Metamask et attendre qu'elle soit terminée

## Comment stake ses sOHM via Etherscan

1. Aller sur dans la section [Write Contract ](https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899#writeContract)du contre OHM.  
  
2. Vérifiez et assurez-vous que le réseau sélectionné est "Ethereum Mainnet" dans votre portefeuille. Appuyez ensuite sur Connect to Web3 pour connecter votre portefeuille si vous ne l'avez pas encore fait.  
  
3. Une fois qu'il est connecté, sélectionnez la troisième option "stake".  
  
4. Dans le champ _\_amount \(uint256\)_, indiquez le montant des OHM que vous souhaitez que le contrat de staking dépense en votre nom, puis multipliez-le par 1e9. Si vous ne voulez pas répéter cette étape à chaque fois que vous voulez miser, vous pouvez choisir une valeur très élevée. Par exemple, pour stake 1 sOHM, saisissez **1'000'000'000**  
  
5. Cliquez sur **Write**.   
  
6. Signez la transaction sur **Metamask** et attendez qu'elle se termine.

