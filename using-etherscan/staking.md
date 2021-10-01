# Stake OHM Anda \(3, 3\)

Terkadang, situs web Olympus mungkin tidak dapat diakses karena[ masalah hosting](https://twitter.com/FleekHQ/status/1416505712222609411) . Jangan takut, Anda masih dapat berinteraksi dengan kontrak Olympus untuk melakukan tindakan tertentu seperti staking. Dalam panduan ini, kami akan menunjukkan caranya agar bisa stake token OHM melalui[ Etherscan](https://etherscan.io/) .

Jika Anda belum pernah mempertaruhkan OHM sebelumnya, ada dua langkah yang harus dilakukan:

1. Setujui kontrak taruhan untuk menggunakan token OHM Anda.
2. Stake token OHM Anda.

Jika Anda telah pernah staking OHM sebelumnya, hanya ada satu langkah yang harus dilakukan: Stake token OHM Anda.

## Bagaimana Cara Menyetujui Penggunaan OHM melalui Etherscan

1. Buka [bagian Kontrak Tulis dari kontrak token OHM](https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899#writeContract).
2. Periksa dan pastikan jaringan yang Anda pilih adalah "Ethereum Mainnet" pada dompet Anda. Kemudian tekan **Hubungkan ke Web3** atau **Connect to Web3** untuk menghubungkan dompet Anda jika Anda belum pernah melakukannya.
3. Setelah terhubung, pilih opsi ketiga "_Approve_" .
4. Di bidang _spender \(address\)_ , kami akan mengisi [alamat kontrak taruhan](https://app.gitbook.com/@olympusdao-1/s/olympusdocs/~/drafts/-MiUWy5CllkavdxoRULJ/v/indonesian/contracts/staking#staking) . Masukkan nilai berikut: **0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d**
5. Pada bidang _amount \(uint256\)_ , isikan jumlah OHM yang Anda inginkan untuk digunakan oleh kontrak taruhan atas nama Anda, dan kalikan dengan 1e9. Atau, Anda dapat menggunakan[ kalkulator ini](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit?usp=sharing) untuk melakukan konversi Anda sendiri. Jika Anda tidak ingin mengulangi langkah ini pada setiap kali Anda ingin staking, Anda dapat memasukkan nilai yang sangat besar. Katakanlah Anda ingin mengizinkan kontrak untuk menggunakan jumlah OHM hingga 1e9 OHM atas nama Anda, Anda bisa memasukkan: **1000000000000000000**
6. Klik Tulis atau **Write**.
7. Tanda tangani transaksi di Metamask dan tunggu sampai selesai.

## Bagaimana Cara Staking OHM melalui Etherscan

1. Pergi ke bagian [Write Contract dari kontrak staking](https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899#writeContract).
2. Periksa dan pastikan jaringan yang Anda pilih adalah "Ethereum Mainnet" pada dompet Anda. Kemudian tekan **Hubungkan ke Web3** atau **Connect to Web3** untuk menghubungkan dompet Anda jika Anda belum melakukannya.
3. Setelah terhubung, pilih opsi "stake".
4. Pada bidang _\_amount \(uint256\)_ , isi jumlah yang ingin Anda pertaruhkan atau stake, dan kalikan dengan 1e9. Atau, Anda dapat menggunakan[ kalkulator ini](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit?usp=sharing) untuk melakukan konversi untuk Anda. Misalnya, jika Anda ingin mempertaruhkan 1 OHM, isikan nilainya: **1000000000**
5. Klik tulis atau **Write**.
6. Tanda tangani transaksi di Metamask dan tunggu sampai selesai.

