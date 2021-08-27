# sOHM 언스테이킹

1. [이더스캔에서 스테이킹 컨트랙트의 'Write Contract'](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a#writeContract) 섹션에 들어갑니다.
2. 지갑에서 연결된 네트워크가 이더리움 메인넷인 것을 확인합니다. 그 후 **Connect to Web3** 버튼을 클릭하여 지갑을 연결해 주세요.
3. 연결 후, _unstake_를 선택합니다.
4. _\_amount \(uint256\)_ 항목에 사용을 허용할 sOHM의 수량에 1e9를 곱한 숫자를 입력해주세요. 계산을 어떻게 해야 할지 확실하지 않으시다면, [본 링크](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit)의 계산기를 사용하시면 됩니다. 예를 들어, 1 sOHM을 언스테이킹 하려면, **1000000000**을 입력하시면 됩니다.
5. _\_trigger \(bool\)_ 항목에 **true**를 입력해주세요.
6. **Write** 버튼을 클릭하세요.
7. 지갑에서 트랜잭션을 승인 후, 완료될 때까지 기다려 주세요.

## 이더스캔을 통해 OHM 스테이킹 하는 법

1. [이더스캔에서 OHM 토큰 컨트랙트의 'Write Contract'](https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f#writeContract) 섹션에 들어갑니다. 
2. 지갑에서 연결된 네트워크가 이더리움 메인넷인 것을 확인합니다. 그 후 **Connect to Web3** 버튼을 클릭하여 지갑을 연결해 주세요.
3. 연결 후, 첫번째 항목인 _approve_를 선택합니다.
4. _spender \(address\)_ 항목에 [스테이킹 컨트랙트](https://docs.olympusdao.finance/references/contracts#staking)의 주소를 입력해 주세요. 주소는 다음과 같습니다:  **0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a**
5. _amount \(uint256\)_ 항목에, 사용을 허용할 sOHM의 수량에 1e9를 곱한 숫자를 입력해주세요. 계산을 어떻게 해야 할지 확실하지 않으시다면, [본 링크](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit)의 계산기를 사용하시면 됩니다. 스테이킹 할 때마다 이 과정을 반복하고 싶지 않으시다면, 큰 숫자를 입력하시면 됩니다. 예를 들어, 컨트랙트에게 1e9 만큼의 sOHM을 사용하게 허용하려면, **1000000000000000000**을 입력하시면 됩니다.
6. **Write** 버튼을 클릭하세요.
7. 지갑에서 트랜잭션을 승인 후, 완료될 때까지 기다려 주세요.

## 이더스캔을 통한 sOHM 사용 승인하는 법 

이전에 sOHM을 언테이킹 하신 적이 있으면, 바로 sOHM 스테이킹을 하실 수 있습니다.

1. sOHM 토큰 사용 승인 
2. sOHM 토큰 스테이킹

sOHM을 전에 언스테이킹 해 보신 적이 없으시다면, 두개의 단계를 거쳐야 합니다:

[호스팅 측](https://twitter.com/FleekHQ/status/1416505712222609411) 문제로 인해 올림푸스 웹사이트가 다운되는 일이 가끔 있을 수 있습니다. 그러나 컨트랙트를 사용하여 언스테이킹 역시 여전히 가능합니다. 이번 가이드에서는 [이더스캔](https://etherscan.io/)을 사용하여 sOHM을 언스테이킹 하는 법을 알아보겠습니다.

