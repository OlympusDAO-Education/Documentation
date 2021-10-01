# Staking

## Distributor

Kontrak distributor menerima OHM yang dicetak dari perbendaharaan untuk memberikan hadiah kepada staker. Target tingkat hadiah pada saat penulisan ditetapkan ke 3500, yang berarti 0,35% dari total suplai, karena tingkat hadiah ditentukan dalam puluhan ribu. Catat bahwa tingkat imbalan menentukan tingkat rebase dan tingkat rebase menentukan APY. Di bawah ini adalah kontrak distributor yang terdaftar berdasarkan versi, di mana versi terbaru mewakili kontrak yang sedang aktif.

* V1 [0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
* V2 [0xce65...f4c4](https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4)
* V3 [0x73cf...bb1e](https://etherscan.io/address/0x73cfe6b116d161a2f9c165f7fc5270fb7dd2bb1e)
* V4 [0xc58e...3ce6](https://etherscan.io/address/0xc58e923bf8a00e4361fe3f4275226a543d7d3ce6)

## Staking LP 

Taruhan LP tidak lagi digunakan. Anda masih dapat melepas LP Anda melalui Etherscan.  


* V1 [0xF11f...2223](https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223)

## Staking

Sebelum migrasi kontrak[ staking,](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2) kontrak[ staking](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2) lama \([ 0x0822...74A2](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2) \) digunakan untuk staking OHM. Jika pengguna masih ada stake di sana, mereka harus memigrasikan OHM yang dipertaruhkan ke kontrak[ taruhan](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a) baru \([ 0xFd31....566a](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a) \). Kontrak[ staking](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d) baru bekerja dengan kontrak[ staking](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d) helper \([ 0xC8C4....612d](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d) \). Kontrak staking helper memilih "stake" dan kemudian "claim" dari kontrak staking baru. Ketika fungsi "stake" dipilih, sOHM dimasukkan ke dalam fase pemanasan dan semua informasi tentang berapa banyak sOHM yang telah dipertaruhkan pengguna disimpan dalam kontrak staking baru. Saat fungsi "klaim" dipilih, sOHM diambil dari pemanasan dan kemudian dikirim ke dompet pengguna.  


