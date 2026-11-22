# Arsip Abyssal

[![make.fun · best-heist-game-20261122-0559](https://make.fun/badge/best-heist-game-20261122-0559.svg)](https://make.fun/bounty/best-heist-game-20261122-0559?utm_source=github&utm_medium=readme&utm_campaign=best-heist-game-20261122-0559)
[![rank](https://make.fun/badge/best-heist-game-20261122-0559/tedinasia/best-heist-game-20261122-0559-v2/rank.svg)](https://make.fun/bounty/best-heist-game-20261122-0559/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=best-heist-game-20261122-0559)
[![reward](https://make.fun/badge/best-heist-game-20261122-0559/tedinasia/best-heist-game-20261122-0559-v2/reward.svg)](https://make.fun/bounty/best-heist-game-20261122-0559?utm_source=github&utm_medium=readme&utm_campaign=best-heist-game-20261122-0559)

Game heist stealth top-down di arsip laut dalam yang bioluminescent. Kamu seorang
penyelam pencuri yang menyusup ke Arsip Abyssal untuk mencuri **Mutiara Abyssal** —
lalu membawanya pulang ke airlock sebelum alarm memuncak.

## Yang membuat entry ini berbeda

- **Tema tidak pasaran:** bukan museum atau bank, melainkan arsip laut dalam.
  Penjaganya ubur-ubur drone mekanik dan kamera "Mata Abyssal" di dinding karang.
- **Semburan Tinta:** charge terbatas. Awan tinta memblokir vision cone guard
  dan kamera selama beberapa detik — jalan keluar saat rute tertutup.
- **Twist — Mutiara Hidup:** begitu Mutiara diambil, ia *hidup* dan bersinar.
  Kamu jadi suar berjalan: guard mengenalimu lebih cepat, cone mereka melebar,
  patroli makin kencang, dan alarm merayap naik sendiri. Pelarian jauh lebih
  berat daripada penyusupan.
- **Identitas visual:** laut dalam navy/teal gelap + cyan bioluminescent untuk
  yang aman, kuning/oranye/merah untuk bahaya, amber hangat untuk loot.
  Sekilas saja sudah jelas mana cover, mana bahaya, mana target.

## Cara main

- **WASD / panah** — bergerak
- **Shift** — jongkok pelan (lebih sulit terlihat)
- **Spasi** — semburan tinta (charge terbatas, +1 tiap mutiara kecil)
- **E** — ambil mutiara kecil / Mutiara Abyssal
- **P** — jeda, **M** — suara hidup/mati, **R** — main lagi setelah menang/kalah
- Klik tombol di layar judul untuk mulai

Bersembunyi di **kelp gelap** (zona "BAYANGAN") membuatmu nyaris tak terlihat.
Deteksi bertahap: guard curiga dulu (cone kuning, tanda "?"), lalu waspada
(cone merah, tanda "!", mengejar posisi terakhirmu). Alarm turun lagi kalau
kamu lolos dari pandangan — tapi kalau mencapai 100%, kamu tertangkap.

Menang: ambil Mutiara Abyssal, lalu kembali ke **Airlock** di kiri bawah.
Mutiara kecil (5) memberi skor dan mengisi tinta.

## Main lokal

```sh
node serve.ts
# buka http://localhost:8080
```

Tidak ada build step, tidak ada network request: semua file statis di `game/`,
suara disintesis lewat WebAudio. Screenshot deterministik tersedia lewat
`?shot=start|play|getaway|win` (lihat `shots.json`).
