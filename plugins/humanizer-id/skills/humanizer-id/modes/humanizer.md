# Mode: Humanizer

> **Kapan dipakai:** ngubah teks yang kaku, formal berlebihan, atau kerasa "AI banget" jadi natural, enak dibaca, dan kayak ditulis manusia beneran.
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
| Register | **Ikutin teks asli dan permintaan user.** Aslinya formal-tapi-boleh-dilonggarin → level 1 |
| Level slang | 1 (naik ke 2 cuma kalau user minta atau teks aslinya emang santai) |
| Kata ganti | `kamu` (atau ikut teks asli) |
| Negasi | `nggak` |
| Singkatan | Ikut teks asli, jangan nambah |
| Emoji | Ikut teks asli, jangan nambah |
| Panjang hasil | ±20% dari teks asli |

---

## Aturan Khusus

### Proses 6 Langkah

1. **Pahami maksud.** Teks ini buat siapa, buat apa, sampai mana batas santainya?
2. **Tandai "AI tells".** Cari frasa klise, kalimat pasif berlapis, dan pembuka/penutup basa-basi (lihat tabel di bawah).
3. **Tentuin Tone Lock.** Level, kata ganti, dan platform. Kalau user nggak bilang, pakai default.
4. **Tulis ulang.**
   - Kalimat aktif dan pendek, variasiin panjangnya.
   - Buang filler yang nggak nambah makna.
   - Terapin tabel ejaan santai di [SKILL.md](../SKILL.md#ejaan-santai-yang-udah-dikunci).
   - Partikel (sih, dong, deh) secukupnya, jangan tiap kalimat.
5. **Cek yang NGGAK boleh berubah:** fakta, angka, tanggal, nama orang/merek, URL, kode, kutipan langsung, istilah teknis.
6. **Output** sesuai format di bawah.

### Aturan Main

- **Jangan nambah info baru.** Humanizer ngubah gaya, bukan isi.
- **Jangan buang poin penting.** Kalau ada bagian yang kepangkas, balikin.
- **Jaga panjang** di kisaran ±20% dari teks asli kecuali user minta lebih ringkas/panjang.
- **Catatan perubahan** (opsional): kalau user minta, kasih daftar singkat apa yang diubah dan kenapa.
- **Jangan ngubah sudut pandang** (misal dari "kami" jadi "gue") kecuali diminta.

### Tabel "AI Tells" Bahasa Indonesia

| ❌ Kerasa AI | ✅ Ganti jadi |
|---|---|
| "Dalam era digital saat ini..." | Langsung ke inti: "Sekarang, hampir semua orang..." |
| "Di dunia yang serba cepat ini..." | Hapus, atau pakai contoh konkret |
| "Penting untuk dicatat bahwa..." | Hapus, langsung sebut poinnya |
| "Tidak dapat dipungkiri bahwa..." | "Jujur aja," / "Emang," |
| "Mari kita selami..." | "Yuk bahas..." / langsung mulai |
| "Bukan hanya X, tetapi juga Y" (berulang) | Sebut X dan Y langsung, variasiin pola |
| "Kesimpulannya," di tiap penutup | Penutup yang punya satu pesan jelas |
| "Semoga bermanfaat!" di tiap akhir | Hapus, atau ganti ajakan yang spesifik |
| "merupakan" di mana-mana | "adalah" / hapus / pakai kata kerja |
| Daftar yang selalu persis 3 item | Sebut sebanyak yang emang ada |
| Tanda pisah panjang (—) di tiap kalimat | Koma, titik, atau pecah kalimat |
| "dapat dilakukan oleh" (pasif berlapis) | "bisa dikerjain" / "kamu bisa..." |
| "sangat", "sekali" ditumpuk | Satu "banget" cukup |
| "Dengan demikian,", "Oleh karena itu," | "Jadi," / "Makanya," |

---

## Struktur dan Format

- **Pertahanin struktur teks asli** (judul, poin, urutan paragraf) kecuali user minta ditata ulang.
- Paragraf panjang boleh dipecah jadi 2–4 kalimat per paragraf.
- List tetap list, tabel tetap tabel.
- Kode, URL, dan kutipan taruh persis seperti aslinya.

---

## Contoh

### Contoh 1 — Paragraf artikel

❌ **Sebelum (kerasa AI):**
> Dalam era digital yang terus berkembang pesat ini, penting bagi kita untuk memahami bahwa manajemen waktu merupakan kunci utama dalam mencapai produktivitas yang optimal. Dengan menerapkan strategi yang tepat, kita dapat menyelesaikan berbagai tugas secara efisien dan efektif.

✅ **Sesudah (level 1):**
> Kalau waktu kamu berantakan, kerjaan ikut berantakan. Makanya ngatur waktu itu penting banget. Tentuin dulu mana yang paling mendesak, kerjain satu-satu, dan sisain waktu buat istirahat.

✅ **Sesudah (level 2):**
> Jujur aja, kerjaan numpuk itu biasanya bukan karena kamu kurang pinter, tapi karena waktunya nggak diatur. Mulai dari yang paling urgent, kerjain satu-satu, dan jangan lupa healing dikit biar nggak burnout.

### Contoh 2 — Deskripsi produk

❌ **Sebelum:**
> Aplikasi ini merupakan solusi inovatif yang dapat membantu pengguna untuk mengelola keuangan pribadi dengan lebih mudah, cepat, dan terstruktur.

✅ **Sesudah (level 1):**
> Aplikasi ini bantu kamu ngatur duit lebih gampang. Catat pengeluaran, liat ke mana aja duitnya lari, beres.

### Contoh 3 — Pesan formal ke tim

❌ **Sebelum:**
> Sehubungan dengan adanya perubahan jadwal, kami mengharapkan kehadiran seluruh anggota tim pada pertemuan yang akan dilaksanakan pada hari Kamis pukul 10.00 WIB.

✅ **Sesudah (level 1):**
> Jadwalnya berubah ya. Rapat tim dipindah ke Kamis jam 10.00 WIB, tolong semua hadir.

> [!NOTE]
> Perhatiin: hari, jam, dan zona waktu **nggak berubah**. Yang diubah cuma gayanya.

---

## Yang Dilarang

- ❌ Ngubah fakta, angka, nama, atau istilah teknis.
- ❌ Nambahin slang tren (🔴) ke teks yang nada aslinya serius.
- ❌ Ngubah teks hukum, kontrak, medis, atau dokumen resmi jadi gaul. Kalau diminta, turunin jadi level 0–1 dan tandai bagian yang sebaiknya tetap baku.
- ❌ Hasil yang nggak konsisten (sebagian `nggak`, sebagian `tidak`).
- ❌ Janji bahwa hasilnya "pasti lolos AI detector". **Nggak ada jaminan itu.**
- ❌ Dipakai buat nyontek tugas akademik atau ngaku-ngaku tulisan orang lain. Tujuan mode ini cuma bikin tulisan lebih enak dibaca.

---

## Checklist

- [ ] Fakta, angka, nama, URL, dan kode nggak berubah?
- [ ] Nggak ada poin penting yang hilang?
- [ ] Nggak ada info baru yang ditambahin?
- [ ] Panjang hasil masih di kisaran ±20%?
- [ ] Frasa "AI tells" udah dibuang?
- [ ] Ejaan konsisten (satu versi `nggak`, `udah`, `aja`)?
- [ ] Level slang sesuai Tone Lock dan konteks?
- [ ] Kalimat pendek dan panjang udah divariasiin?
- [ ] Dibaca keras-keras masih enak?

---

## Format Output

Kasih **hasil rewrite langsung**, tanpa basa-basi pembuka.

```markdown
[teks hasil rewrite]
```

Kalau user minta catatan perubahan, tambahin **di bawah** hasil:

```markdown
**Catatan perubahan:**
- Buang pembuka "Dalam era digital..." (klise).
- Kalimat pasif jadi aktif.
- Level slang: 1, kata ganti: kamu.
```
