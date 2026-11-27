# Mode: Artikel

> **Kapan dipakai:** blog, artikel web, newsletter, caption panjang edukatif, konten edukasi, dan tulisan informatif lain yang pengen enak dibaca (nggak kaku kayak laporan).
> Aturan inti ada di [SKILL.md](../SKILL.md). Kamus kata ada di [kamus-slang.md](../references/kamus-slang.md).

## Daftar Isi

- [Tone Lock Default](#tone-lock-default)
- [Aturan Khusus](#aturan-khusus)
- [Struktur dan Format](#struktur-dan-format)
- [Contoh](#contoh)
- [Yang Dilarang](#yang-dilarang)
- [Checklist](#checklist)
- [Format Output](#format-output)

---

## Tone Lock Default

| Setting | Default |
|---|---|
| Level slang | 1 (level 2 buat blog anak muda/lifestyle) |
| Kata ganti | `kamu` ke pembaca; penulis pakai `aku` atau `kita` (pilih satu) |
| Singkatan | ❌ (tulis lengkap) |
| Emoji | ❌ di isi artikel (newsletter/judul boleh maks 1) |
| Negasi | `nggak` |
| Panjang paragraf | 2–4 kalimat |

---

## Aturan Khusus

- **Fakta tetap akurat.** Santai bukan berarti asal. Cek angka, nama, dan tanggal.
- **Sebut sumber** kalau ada data atau klaim penting.
- **Satu artikel, satu pertanyaan utama.** Jawab itu dengan jelas.
- **Mulai dari yang paling berguna.** Jangan buka dengan sejarah panjang.
- **Contoh konkret** lebih ngena daripada definisi.
- **Keyword SEO masuk natural.** Jangan dijejelin sampai kalimatnya aneh.
- **Santai di cara ngomong, rapi di struktur.** Subjudul, list, dan paragraf pendek tetap dipakai.
- **Slang secukupnya.** Satu-dua kata yang pas, bukan tiap kalimat.

---

## Struktur dan Format

### Artikel / Blog

| Bagian | Isi |
|---|---|
| **Judul** | Catchy tapi jujur (nggak clickbait kosong), memuat keyword utama |
| **Lead** | 2–3 kalimat: masalah/pertanyaan + janji apa yang pembaca dapet |
| **Isi** | Subjudul tiap ±200–300 kata, paragraf 2–4 kalimat, list kalau perlu |
| **Penutup** | Ringkasan singkat + pertanyaan atau CTA |

### Newsletter

| Bagian | Isi |
|---|---|
| **Subject line** | ≤50 karakter, jelas manfaat/penasarannya |
| **Preheader** | 1 kalimat pelengkap |
| **Sapaan** | Personal ("Hai, [nama]") |
| **Isi** | 2–4 bagian pendek, satu bagian = satu ide |
| **CTA** | Satu tombol/link utama |

---

## Contoh

### Contoh 1 — Pembuka artikel

❌ **Kaku:**
> Di era globalisasi seperti sekarang ini, kebutuhan akan pengelolaan keuangan pribadi menjadi sangat penting bagi setiap individu, khususnya generasi muda yang baru memasuki dunia kerja.

✅ **Santai (level 1):**
> Gajian pertama itu seneng banget, sampai tanggal 20 dan kamu baru sadar duitnya lari ke mana. Tenang, hampir semua orang yang baru kerja ngalamin ini. Di artikel ini aku bahas cara ngatur gaji yang gampang dan nggak bikin pusing.

### Contoh 2 — Subjudul dan paragraf

❌ **Kaku:**
> **Pentingnya Dana Darurat**
>
> Dana darurat merupakan sejumlah uang yang disisihkan untuk menghadapi kondisi tidak terduga seperti kehilangan pekerjaan atau kebutuhan medis mendadak.

✅ **Santai (level 1):**
> **Kenapa Kamu Butuh Dana Darurat**
>
> Bayangin tiba-tiba HP rusak, atau kantor tutup bulan depan. Dana darurat itu tabungan khusus buat kejadian kayak gitu, bukan buat beli sepatu diskon. Patokan umumnya, simpen 3–6 kali pengeluaran bulanan.

### Contoh 3 — Subject line newsletter

- ❌ "Newsletter Edisi Bulanan: Informasi Terbaru Seputar Produk Kami"
- ✅ "3 hal yang bikin tabungan kamu nggak nambah-nambah"
- ✅ "Kamu salah sedikit, dan itu wajar"

---

## Yang Dilarang

- ❌ Ngarang data, statistik, atau kutipan.
- ❌ Clickbait yang isinya nggak sesuai judul.
- ❌ Singkatan chat ("yg", "bgt", "gmn") di isi artikel.
- ❌ Emoji bertebaran di isi.
- ❌ Slang tren (🔴) yang bikin artikel cepat basi.
- ❌ Paragraf tembok (lebih dari 5 kalimat).
- ❌ Kalimat pembuka klise ("Di era digital...", "Seiring berkembangnya zaman...").
- ❌ Penutup "Semoga bermanfaat!" yang nggak ada isinya.
- ❌ Keyword stuffing.

---

## Checklist

- [ ] Judul menarik dan jujur?
- [ ] Lead langsung ke masalah dalam 2–3 kalimat?
- [ ] Ada subjudul tiap ±200–300 kata?
- [ ] Paragraf 2–4 kalimat?
- [ ] Fakta dan angka udah dicek, sumber disebut?
- [ ] Nggak ada singkatan chat dan emoji di isi?
- [ ] Penutup ada ringkasan atau CTA?
- [ ] Level slang konsisten dari awal sampai akhir?

---

## Format Output

Kasih artikel dalam format Markdown, **tanpa catatan di dalam isi**:

```markdown
# [Judul]

[Lead]

## [Subjudul 1]

[Isi]

## [Subjudul 2]

[Isi]

## Penutup

[Ringkasan + CTA]
```

Kalau user minta newsletter, tambahin `**Subject:**` dan `**Preheader:**` di atas isi. Catatan ke user (asumsi, data yang perlu dicek) taruh **di luar** blok artikel.
