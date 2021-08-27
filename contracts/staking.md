# 스테이킹

## 배급자\(Distributor\)

배급자 컨트랙트는 금고에서 발행된 OHM을 받아 스테이커들에게 보상을 배분해 줍니다. 보상 비율은 수만 정도로 정의되어 있지만, 현재 작성 시점을 기준으로 그 목표치는 3,500으로 설정되어 있으며 이는 전체 공급량의 0.35%에 해당합니다. 보상 비율이 리베이스 비율이 결정되는데 영향을 끼치며, 그렇게 결정된 리베이스 비율은 APY에 영향을 끼친다는 점을 유념하시길 바랍니다. 아래를 통해 현재 활성화 되어있는 배급자 최신 버전 컨트랙트를 확인하세요.

* V1 [0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
* V2 [0xce65...f4c4](https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4)
* V3 [0x73cf...bb1e](https://etherscan.io/address/0x73cfe6b116d161a2f9c165f7fc5270fb7dd2bb1e)
* V4 [0xc58e...3ce6](https://etherscan.io/address/0xc58e923bf8a00e4361fe3f4275226a543d7d3ce6)

## LP 스테이킹

* V1 [0xF11f...2223](https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223)

## 스테이킹

스테이킹 컨트랙트의 마이그레이션이 있기 이전에, 구 버전의 스테이킹 컨트랙트\([0x0822...74A2](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2)\)가 스테이킹을 위해 사용되었습니다. 만약 그 안에 아직 스테이킹을 하고 있다면, 스테이킹된 OHM을 새로운 스테이킹 컨트랙트\([0xFd31....566a](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a)\) 로 마이그레이션 해야 합니다. 새로운 스테이킹 컨트랙트는 스테이킹 헬퍼 컨트랙트\([0xC8C4....612d](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d)\)와 함께 작동합니다. 스테이킹 헬퍼 컨트랙트는 "stake"를 호출한 뒤 새 스테이킹 컨트랙트를 "claim" 합니다. 스테이크 기능이 호출되면, sOHM은 웜업 단계로 들어가고 유저가 얼마만큼의 sOHM을 스테이킹 하고 있는것인가에 대한 정보가 새로운 스테이킹 컨트랙트에 저장됩니다. "claim" 기능이 호출되면, sOHM은 웜업에서 회수되어 사용자의 지갑으로 전송됩니다.

