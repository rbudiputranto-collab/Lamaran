# Cue Card — Sambutan Lamaran

Kartu sambutan versi web, dioptimalkan untuk dibuka dari HP saat acara berlangsung.
Geser (swipe) kiri/kanan atau ketuk tepi layar untuk pindah kartu.

## Cara deploy ke GitHub Pages (gratis, ±5 menit)

1. Buat repository baru di GitHub, misalnya `sambutan-lamaran`.
   - Bisa **Public** atau **Private** — GitHub Pages tetap bisa jalan untuk keduanya,
     tapi tetap perlu diingat: URL hasil publikasinya nanti **bisa diakses siapa saja
     yang tahu link-nya**, walau repo-nya private. Karena isinya nama lengkap keluarga,
     kalau mau lebih aman, jangan sebar link-nya sembarangan (link tidak akan muncul
     di pencarian Google kecuali sudah diindex).

2. Upload file `index.html` ini ke repo tersebut (lewat "Add file → Upload files" di
   web GitHub, atau lewat `git push` kalau sudah biasa pakai git).

3. Masuk ke **Settings → Pages** di repo tersebut.
   - Di "Build and deployment", pilih **Source: Deploy from a branch**.
   - Branch: `main`, folder `/ (root)` → Save.

4. Tunggu ±1 menit, lalu GitHub akan kasih link seperti:
   `https://<username-anda>.github.io/sambutan-lamaran/`

5. Buka link itu di HP, bisa langsung dipakai. Disarankan "Add to Home Screen"
   dari browser HP supaya bisa dibuka full-screen tanpa address bar, mirip aplikasi.

## Mengubah isi teks

Semua teks kartu ada di bagian atas tag `<script>` dalam `index.html`, di dalam
variabel `CARDS`. Tinggal edit teksnya, simpan, lalu commit/upload ulang ke GitHub —
Pages otomatis update dalam ±1 menit.

Tipe blok yang tersedia per kartu:
- `lead` — kalimat pembuka/penutup yang ditebalkan
- `p` — paragraf biasa
- `pantun` — baris pantun (tampil miring, font serif)
- `direction` — catatan panggung/improvisasi (tampil kecil, warna beda, sebagai pengingat — bukan untuk dibaca apa adanya)
