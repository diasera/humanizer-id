# 🤝 Panduan Kontribusi

Makasih udah mau bantu! Skill ini hidup dari kontribusi orang-orang yang peka sama bahasa sehari-hari. Biar isinya tetap rapi dan konsisten, ikutin panduan singkat ini ya.

---

## Apa Aja yang Bisa Dikontribusiin?

- ➕ **Slang baru** yang lagi kepake.
- ✏️ **Koreksi arti** slang yang kurang pas.
- 🗑️ **Slang basi** yang harus dipindah ke daftar "dilarang" atau labelnya diturunin.
- 📝 **Contoh tulisan** (kaku vs santai) yang lebih bagus, di mode mana pun.
- 🧩 **Mode baru** (lihat bagian [Nambah Mode Baru](#nambah-mode-baru)).
- 🌏 **Variasi daerah** (Jawa, Sunda, Betawi, Medan, dll).
- 🐛 **Typo / format** yang berantakan pas di-render di GitHub.

---

## Format Nambah Slang

Masukin ke tabel yang sesuai di bagian **2. Kamus Slang** di [references/kamus-slang.md](plugins/humanizer-id/skills/humanizer-id/references/kamus-slang.md):

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
2. **Contoh kalimatnya natural**, pakai ejaan santai yang udah dikunci di bagian **Ejaan Santai yang Udah Dikunci** di [SKILL.md](plugins/humanizer-id/skills/humanizer-id/SKILL.md) (`nggak`, `udah`, `aja`, `kayak`).
3. **Nggak dobel** sama yang udah ada.
4. **Nggak dipakai buat ngehina** kelompok tertentu (SARA, body shaming, dll). Kalau istilahnya emang peyoratif, kasih label ⚫ dan catatan.

---

## Nambah Mode Baru

Punya ide mode lain (misal: skrip podcast, caption lowongan kerja, bio marketplace)? Gini caranya:

1. **Copy struktur file mode yang ada** di folder `plugins/humanizer-id/skills/humanizer-id/modes/`. Urutan bagiannya harus sama:
   `Daftar Isi` → `Tone Lock Default` → `Aturan Khusus` → `Struktur dan Format` → `Contoh` → `Yang Dilarang` → `Checklist` → `Format Output`.
2. **Kasih nama file huruf kecil**, pakai strip kalau lebih dari satu kata (contoh: `plugins/humanizer-id/skills/humanizer-id/modes/bio-marketplace.md`).
3. **Minimal 2 pasang contoh** ❌ kaku vs ✅ santai.
4. **Tambah satu baris** di tabel **Pilih Mode** di [SKILL.md](plugins/humanizer-id/skills/humanizer-id/SKILL.md): kapan dipakai, link file, level default, kata ganti default, aturan emoji.
5. **Update tabel mode** di [README.md](README.md) dan catet di [CHANGELOG.md](CHANGELOG.md) bagian *Unreleased*.
6. **Pastiin mode-nya nggak OOT.** Skill ini khusus buat teks Indonesia santai. Mode buat kode, dokumen hukum/medis, atau bahasa lain nggak masuk.

---

## Naikin Versi

Kalau rilis versi baru, update nomor versi yang sama di semua tempat ini:

- `plugins/humanizer-id/plugin.json`
- `plugins/humanizer-id/.codex-plugin/plugin.json`
- `plugins/humanizer-id/.claude-plugin/plugin.json`
- `.claude-plugin/marketplace.json` (2 tempat: `metadata.version` dan `plugins[0].version`)
- `metadata.version` di `plugins/humanizer-id/skills/humanizer-id/SKILL.md`
- Badge versi di `README.md`
- `CHANGELOG.md`

---
## Gaya Nulis di Repo Ini

- Pakai bahasa santai (`gue-lo` / `kamu`), sama kayak isi skill.
- Ikutin ejaan di bagian **Ejaan Santai yang Udah Dikunci** di [SKILL.md](plugins/humanizer-id/skills/humanizer-id/SKILL.md).
- Tabel harus rapi dan tetap ke-render di GitHub (cek tab *Preview* sebelum commit).
- Jangan OOT. Skill ini khusus buat **gaya bahasa Indonesia santai**.
- Pastiin link relatif dan anchor (`#heading`) nggak rusak.

---

## Cara Kirim Kontribusi

1. **Fork** repo ini.
2. Bikin branch baru: `git checkout -b tambah-slang-xyz`
3. Edit file yang sesuai (`references/kamus-slang.md`, `modes/*.md`, atau `SKILL.md`) dan `CHANGELOG.md` di bagian *Unreleased*.
4. Commit dengan pesan yang jelas: `feat: tambah slang "xyz"` / `fix: koreksi arti "abc"` / `feat: tambah mode "xyz"`
5. Buka **Pull Request** dan jelasin singkat perubahannya + sumbernya.

Nggak sempat bikin PR? Buka **Issue** aja, tulis slang + arti + contoh + sumbernya.

---

## Lisensi Kontribusi

Dengan ngirim kontribusi, kamu setuju kontribusimu dirilis di bawah lisensi [MIT](LICENSE) yang sama dengan repo ini.
