# Fuse

Fuse adalah pasar suku bunga terisolasi oleh Rari Capital. Setiap kumpulan (pool) di Fuse dapat mendukung berbagai jenis aset dan menggunakan kurva suku bunga yang berbeda. Untuk meminjamkan sOHM dan/atau menggunakannya sebagai jaminan, pengguna dapat lihat pada[ kolam Olympus Pool Party Fuse](https://app.rari.capital/fuse/pool/18) . Di dalam pool ini, ada beberapa aset didukung:

* sOHM
* USDC
* DAI
* ETH
* FRAX

## Bagaimana Menyuplai Aset

1. Pergi ke[ kolam Olympus Pool Party Fuse](https://app.rari.capital/fuse/pool/18) .
2.  Pada panel Supply, pilih aset yang ingin Anda suplai.

    ![The Supply panel](../../.gitbook/assets/supply.png)
3.  Masukkan jumlah aset yang ingin Anda berikan. Jika Anda ingin menggunakan aset sebagai jaminan untuk meminjam aset lain, aktifkan bidang "Aktifkan Sebagai Jaminan" atau "Enable As Collateral".

    ![Enable as collateral](../../.gitbook/assets/collateral.png)
4. Klik "Konfirmasi" atau "Confirm" . Jika ini adalah pertama kalinya Anda menyuplai aset, Anda harus menyetujui kontrak untuk membelanjakan atau menggunakan aset Anda.
5. Setelah transaksi persetujuan selesai, Anda perlu menandatangani transaksi kedua ke mint fsToken. fsToken mewakili bagian Anda di dalam pool dan memungkinkan Anda untuk menebus aset yang diberikan saat Anda ingin menariknya nanti.
6. Ketika transaksi mint selesai, aset Anda akan dipasok ke Fuse pool. Ini memungkinkan Anda untuk mendapatkan bunga dan juga meminjam aset lain jika Anda telah mengaktifkan aset yang disediakan sebagai jaminan.

Catatan: Jika Anda ingin meminjam aset lain dengan jaminan Anda, ada jumlah pinjaman minimum 1 ETH dengan nilai yang setara. Karena akun kecil mungkin tidak sebanding dengan biaya gas untuk dilikuidasi, ukuran ini memastikan bahwa likuidasi selalu menguntungkan.&#x20;
