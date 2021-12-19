# Stake OHM Anda (3, 3)

Staking memungkinkan Anda untuk mendapatkan OHM secara pasif melalui auto-compounding. Dengan mempertaruhkan OHM Anda dengan OlympusDAO, Anda menerima sOHM (OHM yang dipertaruhkan) sebagai imbalannya dengan rasio 1:1. Setelah itu, saldo sOHM Anda akan meningkat secara otomatis di setiap epoch berdasarkan APY saat ini.

Lihat video ini tentang cara mendapatkan OHM dan mempertaruhkannya (stake) di Olympus:

{% embed url="https://www.youtube.com/watch?v=aXAE1ikVMpM" %}
How to get OHM and stake it on Olympus
{% endembed %}

## Cara Membeli OHM

{% hint style="warning" %}
Ada beberapa tempat untuk membeli OHM: [Sushiswap](https://app.sushi.com/swap), [Uniswap](https://app.uniswap.org/#/swap), or DEX aggregators such as [matcha](https://matcha.xyz). atau agregator DEX seperti [matcha](https://matcha.xyz) . **Pastikan untuk memeriksa slippage terlebih dahulu** sebelum membeli OHM, karena beberapa tempat menawarkan rate yang lebih buruk daripada yang lain karena likuiditas yang rendah.
{% endhint %}

1. Kunjungi [laman Sushiswap swap ini](https://app.sushi.com/swap?outputCurrency=0x383518188c0c6d7730d91b2c03a03c837814a899). Kami menggunakan Sushiswap sebagai contoh di sini. Disarankan untuk membandingkan nilai tukar di berbagai DEX untuk memastikan Anda mendapatkan harga terbaik.
2. Pastikan output mata uang adalah OHM. Anda juga bisa copy dan paste [alamat kontrak OHM](../contracts/tokens.md#ohm) ke bidang output mata uang untuk memastikan Anda menukar mata uang yang tepat.

![Paste OHM contract address](../.gitbook/assets/ohm\_contract.png)

1. Anda dapat memilih mata uang input apa pun berdasarkan saldo dompet yang tersedia. Disarankan untuk menggunakan DAI sebagai mata uang input untuk meminimalisir slippage.

![Make sure the output currency is OHM](../.gitbook/assets/buy\_ohm.png)

1. Pilih jumlah OHM yang ingin Anda tukarkan. Kemudian klik "Setuju" atau "Approve" dan tanda tangani transaksi.
2. Setelah transaksi "Setuju" atau "Approve" berhasil diproses, klik "Tukar" atau "Swap" dan tanda tangani transaksi.
3. Anda akan melihat OHM di saldo dompet Anda sekarang setelah transaksi swap berhasil. Jika Anda tidak dapat menemukannya di dompet Anda, tambahkan [alamat kontrak OHM](../contracts/tokens.md#ohm) pada dompet Anda.

{% hint style="info" %}
Transaksi "Setuju" atau "Approve" hanya diperlukan saat Anda menukar OHM untuk pertama kalinya; swapping berikutnya hanya mengharuskan Anda untuk melakukan transaksi "Swap".
{% endhint %}

## Cara Stake

1. Kunjungi [Stake page of the OlympusDAO website](https://app.olympusdao.finance/#/). Pilih tab "Stake".
2. Masukkan jumlah OHM yang ingin Anda stake di kolom input. Jika Anda ingin men-staking semua saldo OHM Anda yang anda miliki, klik tombol "Max"‚ dan kolom input akan diisi dengan semua saldo OHM Anda yang tersedia.
3. Klik "Approve" dan tanda tangani transaksi.
4. Setelah transaksi "Approve" berhasil diproses, klik "Stake" dan tanda tangani transaksi. Voila, Anda telah mempertaruhkan OHM Anda!

## Cara Unstake

1. Kunjungi [Stake page of the OlympusDAO website](https://app.olympusdao.finance/#/). Pilih tab "Unstake".
2. Masukkan jumlah sOHM yang ingin Anda unstake di kolom input. Jika Anda ingin melepas semua sOHM Anda, tekan tombol "Maks" dan kolom input akan diisi dengan semua saldo sOHM Anda yang tersedia.
3. Klik "Approve" dan tanda tangani transaksi.
4. Setelah transaksi "Approve" berhasil diproses, klik "Unstake" dan tanda tangani transaksi.

Catatan: Transaksi "Approve" hanya diperlukan saat melakukan staking/unstaking untuk pertama kalinya; staking/unstaking berikutnya hanya mengharuskan Anda untuk melakukan transaksi "Stake" atau "Unstake".

## Membaca Info

![The staking page](../.gitbook/assets/staking\_page\_index.png)

**APY** menjelaskan tingkat pengembalian tahunan berdasarkan hasil imbalan. Ini memperhitungkan efek bunga majemuk karena sOHM rebase secara eksponensial.

**TVL** mengukur jumlah dolar dari semua OHM yang distake di Olympus.

**Current Index** atau **Indeks Terkini** memungkinkan Anda untuk melacak keuntungan Anda dari staking. Indeks dimulai dari 1 pada epoch 0, dan meningkat setiap epochnya. Jika Anda staking pada genesis (Epoch 0) dan tidak pernah unstake OHM apa pun, saldo Anda hari ini akan menjadi X kali lebih besar, di mana X adalah indeks saat ini. Anda dapat menggunakan indeks untuk melacak posisi Anda dengan menandai nomor indeks saat Anda stake dan unstake. Anda membagi nomor indeks saat Anda unstake dengan nomor indeks saat Anda stake untuk mendapatkan rasio peningkatan saldo sOHM Anda.

**Your Balance** atau **Saldo Anda** menggambarkan berapa banyak OHM yang tidak di stake di dompet Anda. Ini adalah jumlah maksimum yang dapat Anda stake.

**Your Staked Balance** atau **Saldo Stake Anda** menjelaskan ada berapa banyak staked OHM di dompet Anda. Ini adalah jumlah maksimum yang dapat Anda unstake.

**Next Rebase** memberi tahu Anda waktu yang tersisa hingga rebase berikutnya.

**Reward Yield** Menjelaskan ada berapa banyak saldo sOHM Anda akan meningkat ketika epoch berikutnya dimulai. Misalnya, jika Anda mempertaruhkan 100 OHM dan rebase yang akan datang adalah 0,5427%, saldo sOHM Anda akan meningkat dari 100 menjadi 100,5427.

**ROI (5-Day Rate)** memperkirakan ada berapa banyak saldo sOHM Anda akan meningkat setelah 5 hari, jika hasil imbalan (reward yield) tetap sama selama periode ini. Misalnya, jika Anda memasang 100 OHM dan tarifnya 8,4577%, saldo sOHM Anda akan meningkat dari 100 menjadi 108,4577 setelah 5 hari.
