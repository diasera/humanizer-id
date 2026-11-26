# 🤝 Panduan Kontribusi

Makasih udah mau bantu! Skill ini hidup dari kontribusi orang-orang yang peka sama bahasa sehari-hari. Biar isinya tetap rapi dan konsisten, ikutin panduan singkat ini ya.

---

## Apa Aja yang Bisa Dikontribusiin?

- ➕ **Slang baru** yang lagi kepake.
- ✏️ **Koreksi arti** slang yang kurang pas.
- 🗑️ **Slang basi** yang harus dipindah ke daftar "dilarang" atau labelnya diturunin.
- 📝 **Contoh tulisan** (kaku vs santai) yang lebih bagus.
- 🌏 **Variasi daerah** (Jawa, Sunda, Betawi, Medan, dll).
- 🐛 **Typo / format** yang berantakan pas di-render di GitHub.

---

## Format Nambah Slang

Masukin ke tabel yang sesuai di bagian **6. Kamus Slang Gen Z 2026** di `SKILL.md`:

```markdown
| kata | arti singkat | 🟡 | "Contoh kalimat yang natural." |
```

### Label Umur Kata

| Label | Kapan dipakai |
|---|---|
| 🟢 Evergreen | Udah dipakai bertahun-tahun dan kemungkinan nggak basi. |
| 🟡 Umum | Dipakai luas 1–3 tahun terakhir, dimengerti kebanyakan anak muda. |
| 🔴 Tren | Lagi viral, kemungkinan basi dalam hitungan bulan. |
| ⚫ Kasar | Kasar, vulgar, atau peyoratif. Wajib kasih catatan rating. |

### Syarat Slang Diterima

1. **Artinya jelas** dan bisa dicek di minimal 2 sumber (artikel, postingan, atau pemakaian nyata).
2. **Contoh kalimatnya natural**, pakai ejaan santai yang udah dikunci (`nggak`, `udah`, `aja`, `kayak`).
3. **Nggak dobel** sama yang udah ada.
4. **Nggak dipakai buat ngehina** kelompok tertentu (SARA, body shaming, dll). Kalau istilahnya emang peyoratif, kasih label ⚫ dan catatan.

---

## Gaya Nulis di Repo Ini

- Pakai bahasa santai (`gue-lo` / `kamu`), sama kayak isi skill.
- Ikutin ejaan di bagian **4. Ejaan Santai yang Udah Dikunci**.
- Tabel harus rapi dan tetap ke-render di GitHub (cek tab *Preview* sebelum commit).
- Jangan OOT — skill ini khusus buat **gaya bahasa nulis cerita**.

---

## Cara Kirim Kontribusi

1. **Fork** repo ini.
2. Bikin branch baru: `git checkout -b tambah-slang-xyz`
3. Edit `SKILL.md` (dan `CHANGELOG.md` di bagian *Unreleased*).
4. Commit dengan pesan yang jelas: `feat: tambah slang "xyz"` / `fix: koreksi arti "abc"`
5. Buka **Pull Request** dan jelasin singkat perubahannya + sumbernya.

Nggak sempat bikin PR? Buka **Issue** aja, tulis slang + arti + contoh + sumbernya.

---

## Lisensi Kontribusi

Dengan ngirim kontribusi, kamu setuju kontribusimu dirilis di bawah lisensi [MIT](LICENSE) yang sama dengan repo ini.
