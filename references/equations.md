# Persamaan

## Staking

$$
deposit = withdrawal
$$

Pertukaran antara OHM dan sOHM selama staking dan unstaking selalu dihargai 1:1. Jumlah OHM yang disetorkan ke dalam kontrak staking akan selalu menghasilkan jumlah sOHM yang sama. Dan jumlah sOHM yang ditarik dari kontrak staking akan selalu menghasilkan jumlah OHM yang sama.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

Bendahara menyetorkan OHM ke distributor. Distributor kemudian menyetor OHM ke dalam kontrak staking, sehingga terjadi ketidakseimbangan antara OHM dan sOHM. sOHM di-rebase untuk memperbaiki ketidakseimbangan antara OHM yang disimpan dan sOHM yang beredar. Rebase membawa sOHM yang luar biasa kembali ke paritas sehingga 1 sOHM sama dengan 1 OHM yang dipertaruhkan.

## Bonding

$$
bond Price = 1 + Premium
$$

OHM has an intrinsic value of 1 DAI, whicOHM memiliki nilai intrinsik 1 DAI, yang kira-kira setara dengan $1. Untuk mendapatkan keuntungan dari bonding, Olympus membebankan premi untuk setiap bond.

$$
Premium = debt Ratio * BCV
$$

Premi berasal dari rasio utang sistem dan variabel penskalaan yang disebut [BCV](https://docs.olympusdao.finance/references/glossary#bcv). BCV memungkinkan kita untuk mengontrol tingkat kenaikan harga obligasi.

Premi menentukan keuntungan karena protokol dan pada gilirannya, pemangku kepentingan. Ini karena OHM baru dicetak dari keuntungan dan kemudian didistribusikan di antara semua pemangku kepentingan(staker).

$$
debt Ratio = bondsOutstanding/ohmSupply
$$

Rasio hutang adalah total dari semua OHM yang dijanjikan kepada bonders dibagi dengan total supply OHM. Hal ini memungkinkan kita untuk mengukur hutang sistem.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

Pembayaran obligasi menentukan jumlah OHM yang dijual kepada seorang bonder. Untuk [reserve bonds](https://docs.olympusdao.finance/references/glossary#reserve-bonds), nilai pasar dari aset yang dipasok oleh bonder digunakan untuk menentukan pembayaran obligasi. Misalnya, jika pengguna memasok 1000 DAI dan harga obligasi 250 DAI, pengguna akan mendapatkan 4 OHM.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

Untuk [liquidity bonds](https://docs.olympusdao.finance/references/glossary#liquidity-bonds) , nilai pasar dari token LP yang disediakan oleh bonder digunakan untuk menentukan pembayaran obligasi. Misalnya, jika pengguna memberikan 0,001 OHM-DAI LP token yang bernilai 1000 DAI pada saat bonding, dan harga bond 250 DAI, pengguna akan berhak mendapatkan 4 OHM.

## Pasokan OHM

$$
OHM_{supplyGrowth} = OHM_{stakers} + OHM_{bonders} + OHM_{DAO} + OHM_{pohmExercise}
$$

Suplai atau pasokan OHM tidak memiliki hard cap. Pasokannya meningkan pada saat:

* OHM dicetak dan didistribusikan ke para pemangku kepentingan atau staker.
* OHM dicetak untuk bonder. Ini terjadi setiap kali seseorang membeli obligasi atau bond.
* OHM dicetak untuk DAO. Ini terjadi setiap kali seseorang membeli obligasi. DAO mendapatkan jumlah OHM yang sama dengan bonder.
* OHM dicetak untuk tim, investor, penasihat, atau DAO. Ini terjadi kapan saja pihak tersebut di atas melaksanakan pOHM.

$$
OHM_{stakers} = OHM_{totalSupply} * rewardRate
$$

Pada akhir setiap epoch, perbendaharaan mencetak OHM pada[ tingkat imbalan yang](https://docs.olympusdao.finance/references/glossary#reward-rate) ditetapkan . OHM ini akan didistribusikan ke semua pemangku kepentingan dalam protokol. Anda dapat melacak tingkat hadiah terbaru di[ dasbor Kebijakan Olympus](https://dune.xyz/shadow/Olympus-Policy) .

$$
OHM_{bonders} = bondPayout
$$

Setiap kali seseorang membeli obligasi, sejumlah OHM dicetak. OHM ini tidak akan dilepaskan ke bonder sekaligus - mereka diberikan ke bonder secara linier dari waktu ke waktu. Pembayaran obligasi menggunakan formula yang berbeda untuk berbagai jenis obligasi. Periksa bagian [bagian bond diatas ](equations.md#bonding)untuk melihat cara menghitungnya.&#x20;

$$
OHM_{DAO} = OHM_{bonders}
$$

DAO menerima jumlah OHM yang sama dengan bonder. Ini mewakili keuntungan DAO.

$$
OHM_{pohmExercise} = pOHM + DAI
$$

The individual would supply 1 pOHM along with 1 DAI to mint 1 OHM. The pOHM is subsequently burned. Read [this Medium article](https://olympusdao.medium.com/what-is-poh-16b2c38a6cd6) for more information on pOHM.

## Backing per OHM

$$
OHM_{backing} = treasuryBalance_{stablecoin} + treasuryBalance_{otherAssets}
$$

Setiap OHM yang beredar didukung oleh perbendaharaan Olympus. Aset dalam perbendaharaan dapat dibagi menjadi dua kategori: stablecoin dan non-stablecoin.

$$
treasuryBalance_{stablecoin} = RFV_{reserveBond} + RFV_{lpBond}
$$

Saldo stablecoin di perbendaharaan tumbuh ketika obligasi dijual.  [RFV](https://docs.olympusdao.finance/references/glossary#rfv)  dihitung secara berbeda untuk jenis ikatan yang berbeda.

$$
RFV_{reserveBond} = assetSupplied
$$

Untuk bond cadangan seperti  bond DAI dan bond FRAX, RFV sama dengan jumlah aset dasar yang dipasok oleh bonder.

$$
RFV_{lpBond} = 2sqrt(constantProduct) * (\%\ ownership\ of\ the\ pool)
$$

Untuk bond LP seperti bond OHM-DAI dan bond OHM-FRAX, RFV dihitung secara berbeda karena protokol perlu menurunkan nilainya. Mengapa? Pasangan token LP terdiri dari OHM, dan setiap OHM yang beredar akan didukung oleh token LP ini - ada ketergantungan siklus. Untuk menjamin dengan aman semua OHM yang beredar didukung, protokol menandai nilai token LP ini, maka dinamai nilai bebas risiko atau Risk-Free Value(RFV).
