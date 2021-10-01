# Unstake sOHM

Terkadang, situs web Olympus mungkin tidak dapat diakses karena[ masalah hosting](https://twitter.com/FleekHQ/status/1416505712222609411) . Jangan takut, Anda masih bisa berinteraksi dengan kontrak Olympus untuk melakukan tindakan tertentu seperti unstake. Dalam panduan ini, kami akan menunjukkan kepada Anda cara melepas token sOHM melalui[ Etherscan](https://etherscan.io/) .

Jika Anda belum pernah unstaking sOHM sebelumnya, ada dua langkah yang harus dilakukan:

1. Setujui kontrak taruhan untuk membelanjakan token sOHM Anda.
2. Lepaskan \(unstake\) token sOHM Anda.

Jika Anda sudah pernah unstaking sOHM sebelumnya, hanya ada satu langkah yang harus dilakukan: Unstake token sOHM Anda.

## Bagaimana Cara Menyetujui Penggunaan sOHM melalui Etherscan

1. Buka [bagian Kontrak Tulis dari kontrak token sOHM](https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f#writeContract).
2. Periksa dan pastikan jaringan yang Anda pilih adalah "Ethereum Mainnet" pada dompet Anda. Kemudian tekan **Hubungkan ke Web3** atau **Connect to Web3** untuk menghubungkan dompet Anda jika Anda belum pernah melakukannya.
3. Setelah terhubung, pilih opsi pertama "_approve_" .
4. Di bidang _spender \(address\)_, kami akan mengisi [alamat kontrak stake](https://app.gitbook.com/@olympusdao-1/s/olympusdocs/~/drafts/-MiUWy5CllkavdxoRULJ/v/indonesian/contracts/staking#staking) . Masukkan nilai ini: **0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a**
5. Pada bidang _amount \(uint256\)_ , isi jumlah sOHM yang Anda ingin kontrak stake gunakan atas nama Anda, dan kalikan dengan 1e9. Atau, Anda dapat menggunakan[ kalkulator ini](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit?usp=sharing) untuk melakukan konversi untuk Anda. Jika Anda tidak ingin mengulangi langkah ini setiap kali Anda ingin membatalkan taruhan, Anda bisa memilih nilai yang sangat besar. Katakanlah Anda ingin mengizinkan kontrak menggunakan hingga 1e9 sOHM atas nama Anda, Anda bisa memasukkan**1000000000000000000**
6. Klik Tulis atau **Write**.
7. Tanda tangani transaksi di Metamask dan tunggu sampai selesai.

## Bagaimana Cara Unstake sOHM melalui Etherscan

1. Pergi ke bagian [Write Contract dari kontrak staking](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a#writeContract).
2. Periksa dan pastikan jaringan yang Anda pilih adalah "Ethereum Mainnet" di dompet Anda. Kemudian tekan **Hubungkan ke Web3** untuk menghubungkan dompet Anda jika Anda belum melakukannya.
3. Setelah terhubung, pilih opsi terakhir _unstake_.
4. Pada bidang _\_amount \(uint256\)_ , isi jumlah yang ingin Anda batalkan taruhannya \(unstake\), dan kalikan dengan 1e9. Atau, Anda bisa menggunakan[ kalkulator ini](https://docs.google.com/spreadsheets/d/1vm48OCBnVh8uah0-3Xa7HqFwmfxgcrMIWPrOllSFIvA/edit?usp=sharing) untuk melakukan konversi untuk Anda. Misalnya, jika Anda ingin meng-unstake 1 sOHM, isikan nilainya: **1000000000**
5. Pada kolom _\_trigger \(bool\)_ , isikan nilai: _true_
6. Klik Tulis atau **Write**.
7. Tanda tangani transaksi di Metamask dan tunggu sampai selesai.

