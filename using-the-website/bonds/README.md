# Membeli Obligasi \(bonding\) \(1, 1\)

Bonding memungkinkan pengguna untuk membeli OHM dari protokol dengan harga diskon dengan memperdagangkannya melaui i\) likuiditas \(token LP\) atau ii\) aset lainnya. Yang pertama disebut [bonding likuiditas](https://docs.olympusdao.finance/references/glossary#liquidity-bonds) dan yang kedua disebut [bonding cadangan](https://docs.olympusdao.finance/references/glossary#reserve-bonds) atau bonding aset.

Bonding membutuhkan waktu sekitar 15 epoch untuk bisa diberikan, dan token OHM diberikan secara linier kepada pengguna selama periode tersebut. Bonding likuiditas membantu protokol untuk mengakumulasi dan mengunci likuiditas, sementara bonding cadangan memungkinkan protokol untuk menumbuhkan perbendaharaan, dan dengan demikian RFV-nya lebih cepat.

Olympus menawarkan lima jenis bond atau obligasi di situsnya:

* [Bon DAI](https://app.gitbook.com/@olympusdao-1/s/olympusdocs/~/drafts/-MiUWy5CllkavdxoRULJ/v/indonesian/using-the-website/bonds/bond_dai)
* [Bon FRAX](https://app.gitbook.com/@olympusdao-1/s/olympusdocs/~/drafts/-MiUWy5CllkavdxoRULJ/v/indonesian/using-the-website/bonds/bond_frax)
* [Bon wETH](https://app.gitbook.com/@olympusdao-1/s/olympusdocs/~/drafts/-MiUWy5CllkavdxoRULJ/v/indonesian/using-the-website/bonds/bond_weth)
* [Bon OHM-DAI LP](ohm-dai-lp-bond.md)
* [Bon OHM-FRAX LP](bond_ohm_frax.md)

## Hades

Hades adalah fitur yang memungkinkan Anda untuk membeli obligasi saat mengirim OHM yang diperoleh ke alamat lain. Ini berguna untuk privasi tambahan, atau untuk membeli beberapa bond saat bond saat ini masih vesting. Sebagai catatan bahwa jika akun yang sama memiliki banyak bond, hadiah yang tertunda dari bond sebelumnya harus dibatalkan.

1. Buka [halaman Bond](https://app.olympusdao.finance/#/bonds) dan pilih jenis bond yang ingin Anda beli.
2. Pilih jumlah yang ingin Anda bond, lalu klik ikon roda gigi di kanan atas halaman.

   ![](../../.gitbook/assets/cogwheel.png)

3. Menu Hades akan muncul. Di bagian Recipient Address atau Alamat Penerima, Anda dapat mengisi alamat berbeda untuk menerima OHM saat vesting. Secara default maksudnya bagian itu diisi dengan alamat Anda saat ini.

   ![](../../.gitbook/assets/hades.png)

4. Anda juga dapat memodifikasi bidang slippage untuk menambah atau mengurangi kemungkinan pesanan Anda berhasil. Slippage yang lebih tinggi meningkatkan kemungkinan berhasil lebih besar, tetapi Anda mungkin mendapatkan harga pengisian yang lebih dan tidak diinginkan.
5. Tutup menu Hades dengan mengklik ikon roda gigi lagi.
6. Klik "Setuju" atau "Approve" dan tanda tangani transaksi.
7. Setelah transaksi "Setuju" atau "Approve" berhasil diproses, klik "Bond" dan tanda tangani transaksi. Voila, Anda telah membeli bond pertama Anda menggunakan Hades

_Catatan:_

* Transaksi "Setuju" atau "Approve" hanya diperlukan saat bonding pertama kali; bond berikutnya hanya mengharuskan Anda untuk melakukan transaksi "Bond".
* Saat menggunakan Hades, jangan mengubah jumlah bond setelah Anda menutup menu Hades, karena ini akan mengatur ulang alamat penerima.

## Cara Menukar atau Redeem

Buka [halaman Bond](https://app.olympusdao.finance/#/bonds) dan pilih jenis bond yang telah Anda beli. Pilih tab "Redeem" atau "Tukarkan". Kemudian, klik "Claim Rewards" atau "Klaim Hadiah" untuk mengklaim semua hadiah yang tersedia.

## Membaca Info

![](../../.gitbook/assets/modal.png)

**Balance** adalah saldo token SLP Anda. Ini adalah aset yang digunakan untuk membuat obligasi atau Bond.

**Bond Price** adalah harga OHM yang Anda dapatkan dari bonding. Anda dapat menghitung harga obligasi menggunakan rumus berikut:

* SLP Bond: \(Nilai token SLP Anda / OHM yang akan Anda dapatkan dari bonding\)
* DAI Bond: \(Nilai token DAI Anda / OHM yang akan Anda dapatkan dari bonding\)

**Market Price** adalah harga pasar OHM.

**You Will Get** memberi tahu Anda berapa banyak OHM yang akan Anda dapatkan dari bonding.

**Debt Ratio** mengukur jumlah total OHM yang dibuat dari obligasi yang belum dibayarkan oleh protokol. Rasio utang dihitung secara berbeda untuk obligasi SLP dan obligasi DAI:

* SLP Bond: \(OHM dibuat dari bond yang belum ditukarkan / total suplai OHM\)
* DAI Bond: \(OHM dibuat dari bond yang tidak ditukarkan / suplai OHM yang beredar\)

**Vesting Term** mengukur periode yang diperlukan satu bond untuk ditukarkan sepenuhnya. Angka periode ini tertera di blok Ethereum. Untuk 33110 blok adalah sekitar 5 hari atau 15 epoch.

**Discount** adalah selisih antara harga obligasi dan harga pasar. Pada tangkapan layar di atas, bonding akan memberi Anda diskon 10,63% dibandingkan membeli OHM dalam jumlah yang sama dari pasar.

![](../../.gitbook/assets/modal_redeem.png)

**Pending Rewards** adalah jumlah OHM yang berhak Anda terima dari bonding.

**Claimable Rewards** adalah jumlah OHM yang bisa kamu claim sekarang. Jumlah ini terus meningkat karena OHM terus divesting kepada Anda selama periode bonding.

**Full Bond Maturation** mengacu pada blok Ethereum ketika obligasi dapat ditukarkan sepenuhnya.

