# REPORT — bring-the-humans-02 "Bring the humans again" (fresh build)

## Entry

- **Repo:** `~/workspace/makefun/bring-the-humans-02-fresh/` (local only — belum di-push, belum di-submit; itu kerjaan main agent)
- **Anchor:** `makefun anchor 4adbeaaa1bb75f067255459dc634929a2821ab70 round 34066347` (dicetak sebagai aksi pertama sesi ini, sebelum menulis apa pun — kit init di repo baru)
- **Files:** `README.md` (7.695 byte), `screenshot.png` (590.218 byte, 1100×3356 = 3.691.600 piksel), `LICENSE` (MIT, dari kit init)

## Isi guide

README.md mengikuti template requirements PERSIS: judul `# bring-the-humans-02`, 3 badge live (slug + rank + reward, owner kingwolf-byte), deskripsi, seksi `## Run it` (`python3 -m http.server 8000`), footer `Entered on make.fun ?ref=z2v3hcxy`. Tidak ada placeholder `{…}` tersisa; tidak ada `.github/README.md`.

Isi guide (Bahasa Inggris, jujur, meyakinkan tanpa melebih-lebihkan), ditulis fresh di sesi ini:

1. **What is make.fun?** — marketplace tempat AI agents build software for cash rewards, dibayar USDC di Solana.
2. **How it works** — 4 langkah: sign up → pick a bounty → agent builds → graded & paid.
3. **Sign up** — link referral **https://make.fun/r/z2v3hcxy** (kode `z2v3hcxy`) ditampilkan tebal sebagai satu-satunya CTA, plus syarat wallet Solana + GitHub, dengan penekanan: wallet yang dihubungkan saat signup adalah wallet payout (cek alamatnya), dan owner repo harus cocok dengan akun GitHub yang terhubung.
4. **What can your agent build?** — games, trading/forecasting bots, data tools, creative work, guides/ads.
5. **How prizes work** — pool $1.000 ($150/$80/$50, lalu $20/$17/$13 sampai rank 50), klaim sendiri setelah hasil diumumkan.
6. **What does it cost?** — mayoritas bounty gratis; sebagian kecil berbayar dan selalu ditampilkan di depan.
7. **Honest expectations** — hadiah kompetitif bukan jaminan, bukan passive income, kualitas > kuantitas, jangan pernah bagi seed phrase.
8. **Tips from someone already competing** — mulai dari field kecil, baca leaderboard top 5 dulu, cek requirements endpoint, jangan kejar bounty yang sudah cap reputasi, simpan transcript, resubmit hanya kalau lebih baik, plus tip khusus bounty referral: distribusi adalah skornya — share di tempat yang dilihat pemilik agen AI sungguhan, dan jangan pernah memalsukan signup.
9. **FAQ** — perlu coding? (tidak), perlu bayar? (tidak), cara dibayar, satu agen per entry, kalau skor nol itu normal.

Struktur ini dipilih karena skor kompetisi ini = signup manusia beneran lewat referral link. Pembaca harus (a) paham apa itu make.fun dalam 30 detik, (b) percaya ini legit (jujur soal odds, bukan janji penghasilan), (c) punya satu aksi jelas: klik link referral. Bagian "Honest expectations" sengaja ditaruh sebelum tips — kepercayaan lebih penting daripada hype untuk mengubah pembaca jadi pendaftar.

## Screenshot

`screenshot.png` adalah render penuh README via Playwright (Chromium-1255, viewport 1100, fullPage, 0 console error). Ketiga badge live diunduh via curl dan di-inline sebagai data URI di HTML render saja (README.md tetap memakai URL live; di GitHub badge akan tampil normal). Hasil akhir: 3 badge tampil ("make.fun bring-the-humans-02", "rank 348 entries · closes Nov 21", "pool $1,000 USDC"), seluruh teks terbaca, link referral terlihat jelas. Ukuran 1100×3356 (3.691.600 piksel < batas 16 juta), 590.218 byte (< batas 8 MB). Dibaca visual langsung oleh coordinator: rapi, tidak ada overflow, footer "Entered on make.fun" tampil.

## Verifikasi

- `grep z2v3hcxy README.md` → 3 kemunculan (link /r/z2v3hcxy, kode dalam teks, footer ?ref=z2v3hcxy).
- `grep "{...}" README.md` → tidak ada placeholder tersisa.
- 3 badge `badge/bring-the-humans-02` ada di README.
- Tidak ada `.github/` di repo.
- README 7.695 byte (< 2 MB), screenshot 590.218 byte (< 8 MB) dan 3.691.600 piksel (< 16 juta).
- thinking_revised: README ditulis lalu 2 edit genuine di message terpisah (penjelasan wallet payout + owner repo di seksi Sign up; tip distribusi di seksi Tips).

## Verdict jujur soal odds

Puncak TIPIS tapi field membesar cepat: 334 entry di 18:44 WIB, 348 entry saat badge diunduh ~18:47 WIB; rank 1 baru 3 signup provisional (0 verified). Top 1 secara angka cuma butuh 4+ signup beneran — jauh lebih terjangkau daripada -01. TAPI skor = distribusi link, bukan kualitas halaman. Guide sebagus apa pun tidak menghasilkan signup sendiri; yang menentukan adalah apakah link referral disebar ke manusia sungguhan yang punya agen AI dan mau daftar. Tanpa distribusi, entry ini hampir pasti berakhir 0 signup. Dengan distribusi, top 1–5 realistis karena puncak masih tipis. Jangan pernah memalsukan signup — itu melanggar aturan dan bisa didiskualifikasi.
