# Persamaan

## Staking

$$
deposit = withdrawal
$$

Pertukaran antara OHM dan sOHM selama staking dan unstaking selalu dinilai dengan perbandingan 1:1. Jumlah OHM yang disetorkan ke dalam kontrak staking akan selalu menghasilkan jumlah sOHM yang sama. Dan jumlah sOHM yang ditarik dari kontrak staking akan selalu menghasilkan jumlah OHM yang sama.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

Bendahara menyetorkan OHM ke distributor. Distributor kemudian menyetor OHM ke dalam kontrak staking, sehingga terjadi ketidakseimbangan antara OHM dan sOHM. sOHM di-rebase untuk memperbaiki ketidakseimbangan antara OHM yang tersimpan dan sOHM yang beredar. Rebase membawa sOHM yang luar biasa kembali ke paritas sehingga 1 sOHM sama dengan 1 OHM yang distake.

## Bonding

$$
bond Price = 1 + Premium
$$

OHM memiliki nilai intrinsik 1 DAI, yang kira-kira setara dengan $1. Untuk mendapatkan keuntungan dari bonding, Olympus membebankan premi untuk setiap bond.

$$
Premium = debt Ratio * BCV
$$

Premi berasal dari rasio utang sistem dan variabel penskalaan yang disebut[ BCV](https://docs.olympusdao.finance/references/glossary#bcv). BCV memungkinkan kita untuk mengontrol tingkat kenaikan harga obligasi.

Premi menentukan hak laba untuk protokol dan juga staker. Ini karena OHM yang baru dicetak dari laba dan kemudian didistribusikan di antara semua staker.

$$
debt Ratio = bondsOutstanding/ohmSupply
$$

Rasio hutang adalah total dari semua OHM yang dijanjikan kepada bonder dibagi dengan total supplai OHM. Hal ini memungkinkan kita untuk mengukur hutang sistem.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

Pembayaran bond menentukan jumlah OHM yang dijual kepada seorang bonder. Untuk[ ](https://docs.olympusdao.finance/references/glossary#reserve-bonds)[**reserve bonds**](https://docs.olympusdao.finance/references/glossary#reserve-bonds) , nilai pasar dari aset yang disuplai oleh bonder digunakan untuk menentukan pembayaran bond. Misalnya, jika pengguna memasok 1000 DAI dan harga bond 250 DAI, pengguna akan mendapatkan 4 OHM.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

Untuk [liquidity bonds](https://docs.olympusdao.finance/references/glossary#liquidity-bonds) , nilai pasar dari token LP yang disediakan oleh bonder digunakan untuk menentukan pembayaran bond. Misalnya, jika pengguna memberikan 0,001 OHM-DAI LP token yang bernilai 1000 DAI pada saat bonding, dan harga bond 250 DAI, pengguna akan berhak mendapatkan 4 OHM.

## OHM Supply

$$
OHM_{supplyGrowth} = OHM_{stakers} + OHM_{bonders} + OHM_{DAO}
$$

Suplai OHM tidak memiliki hard cap atau batasan tertinggi. Suplainya meningkat ketika:

* OHM dicetak dan didistribusikan ke para staker.
* OHM dicetak untuk bonder. Ini bisa kapan saja ketika seseorang membeli obligasi.
* OHM dicetak untuk DAO. Ini terjadi setiap kali seseorang membeli obligasi atau bond. DAO mendapatkan jumlah OHM yang sama dengan bonder.
* OHM dicetak untuk tim, investor, penasihat, atau DAO itu sendiri. Ini terjadi setiap kali ketika pihak tersebut di atas melaksanakan pOHM.

$$
OHM_{stakers} = OHM_{totalSupply} * rewardRate
$$

Pada akhir setiap epoch, perbendaharaan mencetak OHM pada[ tingkat imbalan yang](https://docs.olympusdao.finance/references/glossary#reward-rate) ditetapkan . OHM ini akan didistribusikan ke semua staker dalam protokol. Anda dapat melacak tingkat hadiah terbaru di[ dasbor Kebijakan Olympus](https://dune.xyz/shadow/Olympus-Policy).

$$
OHM_{bonders} = bondPayout
$$

Setiap kali seseorang membeli bond, sejumlah OHM akan dicetak. OHM ini tidak akan dilepaskan kepada bonder sekaligus - mereka akan diberikan ke bonder secara linier dari waktu ke waktu. Pembayaran bond menggunakan formula yang berbeda untuk berbagai jenis bond. Periksa bagian [bond di atas](https://docs.olympusdao.finance/main/references/equations#bonding) untuk melihat cara menghitungnya.

$$
OHM_{DAO} = OHM_{bonders}
$$

DAO menerima jumlah OHM yang sama dengan bonder. Ini mewakili keuntungan DAO.

## Dukungan per OHM

$$
OHM_{backing} = treasuryBalance_{stablecoin} + treasuryBalance_{otherAssets}
$$

Setiap OHM yang beredar didukung oleh perbendaharaan Olympus. Aset dalam perbendaharaan dapat dibagi menjadi dua kategori: stablecoin dan non-stablecoin.

$$
treasuryBalance_{stablecoin} = RFV_{reserveBond} + RFV_{lpBond}
$$

Saldo stablecoin di perbendaharaan bertambah ketika bond terjual.[ RFV](https://docs.olympusdao.finance/references/glossary#rfv) dihitung secara berbeda untuk jenis bond yang berbeda.

$$
RFV_{reserveBond} = assetSupplied
$$

Untuk bond cadangan seperti bond DAI dan bond FRAX, RFV sama dengan jumlah aset dasar yang disuplai oleh bonder.

$$
RFV_{lpBond} = 2sqrt(constantProduct) * (\%\ ownership\ of\ the\ pool)
$$

Untuk bond LP seperti bond OHM-DAI dan bond OHM-FRAX, RFV dihitung secara berbeda karena protokol perlu menurunkan nilainya. Mengapa? Pasangan token LP terdiri dari OHM, dan setiap OHM yang beredar akan dicadangkan oleh token LP ini - ada ketergantungan siklus terjadi disini. Untuk menjamin dengan aman semua OHM yang beredar tercadangkan, protokol menandai nilai token LP ini, maka dari itulah bernama nilai bebas risiko atau _Risk-Free Value_ \(RFV\).  


