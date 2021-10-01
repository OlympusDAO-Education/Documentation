# Stake OHM Anda \(3, 3\)

Staking memungkinkan Anda untuk mendapatkan OHM secara pasif melalui auto-compounding. Dengan mempertaruhkan OHM Anda dengan OlympusDAO, Anda menerima sOHM \(OHM yang dipertaruhkan\) sebagai imbalannya dengan rasio 1:1. Setelah itu, saldo sOHM Anda akan meningkat secara otomatis di setiap epoch berdasarkan APY saat ini.

Lihat video ini tentang cara mendapatkan OHM dan mempertaruhkannya di Olympus:

{% embed url="https://www.youtube.com/watch?v=aXAE1ikVMpM" caption="" %}

## Cara Membeli OHM

Ada beberapa tempat untuk membeli OHM:[ Sushiswap](https://app.sushi.com/swap) , Uniswap , atau agregator DEX seperti[ matcha](https://matcha.xyz/) . Pastikan untuk memeriksa slippage terlebih dahulu sebelum membeli OHM, karena beberapa tempat menawarkan rate yang lebih buruk daripada yang lain karena likuiditas yang rendah.

1. Buka[ halaman swap Sushiswap ini](https://app.sushi.com/swap?outputCurrency=0x383518188c0c6d7730d91b2c03a03c837814a899).

2. Pastikan mata uang keluaran adalah OHM. Anda juga dapat menyalin dan menempelkan [alamat kontrak OHM](https://docs.olympusdao.finance/contracts/tokens) ke bidang mata uang keluaran untuk memastikan Anda menukar token yang tepat.

![Paste OHM contract address](../.gitbook/assets/ohm_contract.png)

3. Anda dapat memilih mata uang input apa pun berdasarkan saldo dompet yang tersedia. Disarankan untuk menggunakan DAI sebagai mata uang input untuk meminimalisir slippage.

![Make sure the output currency is OHM](../.gitbook/assets/buy_ohm.png)

4. Pilih jumlah OHM yang ingin Anda tukarkan. Kemudian klik "Setuju" atau "Approve" dan tanda tangani transaksi.

5. Setelah transaksi "Setuju" atau "Approve" berhasil diproses, klik "Tukar" atau "Swap" dan tanda tangani transaksi.

6. Anda akan melihat OHM di saldo dompet Anda sekarang setelah transaksi swap berhasil. Jika Anda tidak dapat menemukannya di dompet Anda, tambahkan [alamat kontrak OHM](https://docs.olympusdao.finance/contracts/tokens) ke dompet Anda.

_Catatan: Transaksi "Setuju" atau "Approve" hanya diperlukan saat Anda menukar OHM untuk pertama kalinya; swapping berikutnya hanya mengharuskan Anda untuk melakukan transaksi "Swap"._

## Bagaimana cara Staking?

1. Buka halaman [Stake di situs web OlympusDAO](https://app.olympusdao.finance/#/stake) . Pilih tab "Stake".
2. Masukkan jumlah OHM yang ingin Anda stake di kolom input. Jika Anda ingin men-staking semua saldo OHM Anda yang anda miliki, klik tombol "Max"‚ dan kolom input akan diisi dengan semua saldo OHM Anda yang tersedia.
3. Klik "Approve" dan tanda tangani transaksi.
4. Setelah transaksi "Approve" berhasil diproses, klik "Stake" dan tanda tangani transaksi. Voila, Anda telah mempertaruhkan OHM Anda!

 _Catatan: Jika kamu tidak melihat sOHM di dompetmu, kamu bisa menambahkannya ke dalam dompetmu dengan_ [_alamat kontrak sOHM_](https://docs.olympusdao.finance/contracts/tokens)_._

## Cara Unstake

1. Buka [halaman Taruhan di situs web OlympusDAO](https://app.olympusdao.finance/#/stake) . Pilih tab "Unstake".
2. Masukkan jumlah sOHM yang ingin Anda unstake di kolom input. Jika Anda ingin melepas semua sOHM Anda, tekan tombol "Maks" dan kolom input akan diisi dengan semua saldo sOHM Anda yang tersedia.
3. Klik "Approve" dan tanda tangani transaksi.
4. Setelah transaksi "Approve" berhasil diproses, klik "Unstake" dan tanda tangani transaksi.

_Catatan: Transaksi "Approve" hanya diperlukan saat melakukan staking/unstaking untuk pertama kalinya; staking/unstaking berikutnya hanya mengharuskan Anda untuk melakukan transaksi "Stake" atau "Unstake"._

## Reading the Info

![The staking page](../.gitbook/assets/staking_page_index.png)

**APY** menjelaskan tingkat pengembalian tahunan berdasarkan hasil imbalan. Ini memperhitungkan efek bunga majemuk karena sOHM rebase secara eksponensial.

**TVL** mengukur jumlah dolar dari semua OHM yang distake di Olympus.

**Indeks saat ini** atau **Current Index** memungkinkan Anda untuk melacak keuntungan Anda dari staking. Indeks dimulai dari 1 pada epoch 0, dan meningkat setiap epochnya. Jika Anda staking pada genesis \(Epoch 0\) dan tidak pernah unstake OHM apa pun, saldo Anda hari ini akan menjadi X kali lebih besar, di mana X adalah indeks saat ini. Anda dapat menggunakan indeks untuk melacak posisi Anda dengan menandai nomor indeks saat Anda stake dan unstake. Anda membagi nomor indeks saat Anda unstake dengan nomor indeks saat Anda stake untuk mendapatkan rasio peningkatan saldo sOHM Anda.

**Saldo Anda** atau **Your Balance** menggambarkan berapa banyak OHM yang tidak di stake di dompet Anda. Ini adalah jumlah maksimum yang dapat Anda stake..

**Saldo Taruhan Anda** atau **Your Staked Balance** menjelaskan ada berapa banyak staked OHM di dompet Anda. Ini adalah jumlah maksimum yang dapat Anda unstake.

**Next Rebase** memberi tahu Anda waktu yang tersisa hingga rebase berikutnya.

Reward Yield Menjelaskan ada berapa banyak saldo sOHM Anda akan meningkat ketika epoch berikutnya dimulai. Misalnya, jika Anda mempertaruhkan 100 OHM dan rebase yang akan datang adalah 0,5427%, saldo sOHM Anda akan meningkat dari 100 menjadi 100.5427.

**ROI \(Tarif 5 Hari\)** memperkirakan ada berapa banyak saldo sOHM Anda akan meningkat setelah 5 hari, jika hasil imbalan \(reward yield\) tetap sama selama periode ini. Misalnya, jika Anda memasang 100 OHM dan tarifnya 8,4577%, saldo sOHM Anda akan meningkat dari 100 menjadi 108,4577 setelah 5 hari.

