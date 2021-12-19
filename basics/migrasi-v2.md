# Migrasi V2

## **Mengapa saya perlu bermigrasi?**

V2Migrasi V2 memperkenalkan fitur-fitur baru seperti tata kelola on-chain dan auto-staking untuk bond.

Transisi dari sOHM V1 ke gOHM memungkinkan beberapa bond diambil pada saat yang bersamaan atau satu waktu, yang mana sebelumnya bertolak-belakang, yaitu satu bond saja per periode vesting.

Sebagian dari likuiditas akan tetap ada untuk v1 OHM saat proses migrasi berlangsung. Hal ini memberikan likuiditas yang cukup bagi peminjam untuk menutup atau memindahkan posisi pinjaman mereka.

Anda dapat membaca lebih lanjut tentang ini di halaman [Olympus Medium](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe) .

{% hint style="info" %}
Anda memiliki waktu **dua bulan untuk bermigrasi setelah peluncuran V2.** Jika dalam kurun waktu tersebut Anda tidak melakukannya, saldo sOHM V1 Anda akan berhenti melakukan rebasing, tetapi berbeda jika anda Anda bermigrasi, ia akan tetap rebasing.
{% endhint %}

{% hint style="info" %}
Pada artikel ini, kami menambahkan V1 dan V2 setelah setiap nama token untuk membantu Anda membedakan antara token lama dan baru. Pada situs web mitra, agregator harga, atau dompet Anda tidak akan menampilkan informasi versi token
{% endhint %}

## Apa TLDR-nya?

* wsOHM V1 (wrapped, staked OHM) akan digantikan oleh gOHM (Governance OHM). Mereka berfungsi sama persis, tetapi gOHM diatur untuk tata kelola on-chain.
* Token OHM dan sOHM akan memiliki rekan V2 yang identik. OHM V1 menjadi OHM V2, dan sOHM V1 menjadi sOHM V2.
* Ticker token akan tetap sama untuk token V1. Misalnya, setelah migrasi, dompet Anda akan menampilkan "OHM" bukan "OHM V1". Pastikan untuk memperbarui kontrak token di dompet Anda dengan [V2 addresses](../contracts/tokens.md)  untuk melihat saldo Anda.
* Saat memigrasikan OHM V1 dan/atau sOHM V1, Anda akan mendapatkan gOHM sebagai gantinya. Meskipun saldo token akan berbeda (harga gOHM dihitung secara berbeda, yang didasarkan pada Indeks Terkini), **jumlah dolar tetap sama.**
* Setelah migrasi, kumpulan OHM V1 seperti OHM-DAI akan menggunakan OHM V2. Ini juga berlaku untuk bond yang baru. Mitra seperti Abracadabra hanya akan menerima setoran baru dalam bentuk gOHM. Jadi, Anda perlu bermigrasi jika ingin menggunakan fitur ini. Jika tidak, Anda dapat duduk diam dan bermigrasi hanya jika Anda mau.

## **Bagaimana jika saya tidak bermigrasi?**

Anda tidak bisa menikmati fitur-fitur baru yang diperkenalkan oleh V2. Beberapa mitra seperti Rari Capital hanya akan menerima token V2 kedepannya, jadi Anda perlu bermigrasi jika ingin menggunakan lebih banyak token (misalnya membuat deposit baru) di platform ini.

## **Seumpama biaya gas sedang tinggi, apakah saya akan kehilangan hadiah rebase saya jika saya menunda migrasi?**

Tidak, Anda dapat bermigrasi sesuka hati setelah diterbitkan. Smart Contract akan melacak hadiah rebase yang berhak Anda miliki sehingga Anda tidak akan melewatkannya sedikitpun.

## **Bagaimana proses migrasinya?**

Saat migrasi aktif, front-end Olympus akan diperbarui untuk me-migrasikan semua token V1 Anda (yaitu OHM, sOHM, dan wsOHM) menjadi gOHM.

Proses migrasi itu sendiri memerlukan dua langkah: satu untuk menyetujui kontrak pada setiap token V1 Anda, dan satu lagi yang benar-benar memigrasikan semua token Anda ke gOHM.

{% hint style="info" %}
Setiap jenis token V1 memerlukan langkah persetujuannya sendiri. Misalnya, jika Anda memiliki OHM V1 dan sOHM V1 di dompet Anda, Anda perlu melakukan dua persetujuan token, tetapi hanya satu operasi migrasi (keseluruhannya menjadi tiga transaksi).
{% endhint %}

## **Bisakah saya memigrasikan jenis token V1 tertentu dan menyisakan sebagian lainnya?**

Tidak. Anda harus memigrasikan semua token V1 Anda (yaitu OHM, sOHM, dan wsOHM) atau tidak sama sekali.

## **Bisakah saya beralih kembali ke token V1 setelah memigrasikannya ke gOHM?**

No, yoTidak, Anda tidak dapat beralih kembali dari token gOHM ke V1 melalui alat migrasi kami.

## **Bisakah Anda memberikan contoh seberapa banyak gOHM yang bisa saya dapatkan dari migrasi?**

Dengan asumsi Anda memiliki 20 OHM V1, 20 sOHM V1, dan 20 wsOHM, dan [Indeks Terkini](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards) adalah 10.

* 20 OHM V1 = 2 gOHM. Ambil 20 OHM Anda dan bagi dengan Indeks Terkini untuk mendapatkan gOHM Anda.
* 20 sOHM V1 = 2 gOHM. Ambil 20 sOHM Anda dan bagi dengan Indeks Saat Ini untuk mendapatkan gOHM Anda.
* 20 wsOHM = 20 gOHM. 1 wsOHM setara dengan 1 gOHM.

{% hint style="info" %}
Sebagai pengingat, jika Anda bermigrasi dari token berbasis non-indeks (OHM, sOHM) ke token berbasis indeks (gOHM), Anda tidak akan menerima jumlah token yang sama setelah migrasi, tetapi masih bernilai sama dalam istilah dolar.&#x20;
{% endhint %}

## **Apakah gOHM saya masih mendapatkan imbalan rebase?**

Ya. Meskipun gOHM tidak berubah dalam kuantitas setelah rebase seperti halnya sOHM, namun anda tetap mendapatkan imbalan rebase. Hal ini karena harga gOHM terkait dengan Indeks Terkini:

$$
gOHM_{price} = OHM_{price} * CurrentIndex
$$

Setiap event rebase akan menyebabkan Current Index (Indeks Terkini) naik, dan gOHM Anda lebih bernilai sebagai gantinya (asalkan harga OHM tetap konstan).

## **Bagaimana pengaruhnya terhadap Bond setelah migrasi?**

In V2, you can purchase multiple bonds of the same type without resetting the bond vesting period. Di V2, Anda dapat membeli beberapa bond dengan jenis yang sama tanpa mengatur ulang periode vesting bond.

Selain itu, tidak perlu lagi mengklaim imbalan bond dan staking ulang secara manual, karena proses ini akan terjadi otomatis. Bonder akan menerima sOHM nya pada akhir periode vesting.

Pelajari lebih lanjut tentang bagaimana perilaku bond di V2 dari halaman [Olympus Medium](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe) .

## **Apakah Olympus V2 sudah diaudit?**

Semua kontrak terkait V2 sudah aktif, dan beberapa di antaranya masih dalam proses audit. Kami bekerja dengan Runtime Verification untuk audit, dan hasilnya akan dipublikasikan begitu ia tersedia.
