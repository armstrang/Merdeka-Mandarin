# Merdeka Mandarin

Aplikasi belajar kosakata HSK 1–6 (silabus HSK 3.0, terbit November 2025): daftar kata, kartu hafalan, kuis, dan progres pemahaman per kata. Berjalan sepenuhnya offline.

## Pasang di Android

1. Buka halaman **[Releases](../../releases/latest)** dari HP.
2. Unduh `MerdekaMandarin.apk`.
3. Buka file itu. Jika diminta, izinkan "Instal aplikasi tidak dikenal" untuk browser atau file manager yang dipakai.

Versi baru dipasang dengan cara yang sama, langsung di atas versi lama. Progres belajar tidak hilang.

## Cara kerja

- Halaman aplikasinya ada di `app/src/main/assets/index.html` (satu file HTML berisi semua data kosakata).
- Setiap kali ada perubahan di branch `main`, GitHub Actions membangun APK dan menerbitkannya di Releases.
- APK ditandatangani dengan kunci di `keystore/` supaya setiap versi bisa memperbarui versi sebelumnya.

## Sumber data

Daftar kata dan pinyin dari [harukicoder/hsk30](https://github.com/harukicoder/hsk30). Arti, contoh kalimat, dan terjemahannya ditulis oleh Claude.

## Versi 1.5-V2 (Liquid Glass)

Opsi tampilan kedua bergaya *Liquid Glass*: kaca buram transparan, latar warna yang bergerak pelan,
animasi transisi yang halus, dan getar ringan saat menjawab. Unduh **MerdekaMandarin-V2.apk** dari
rilis [v1.5-V2](../../releases/tag/v1.5-V2). Aplikasinya bernama **Merdeka Mandarin V2** dan bisa dipasang
berdampingan dengan aplikasi utama; progres belajar keduanya terpisah.

Struktur: `app/src/classic/assets/index.html` (aplikasi utama) dan `app/src/glass/assets/index.html` (V2).
