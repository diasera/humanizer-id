# Mode: Cerita

> **Kapan dipakai:** nulis, ngelanjutin, ngedit, atau nge-review cerita fiksi: Wattpad, novel online, cerbung, AU, fanfic (bab, prolog, dialog, chat scene, blurb, author's note).
> Aturan inti (ejaan, partikel, level slang, peka konteks) ada di [SKILL.md](../SKILL.md). Kamus kata ada di [kamus-slang.md](../references/kamus-slang.md).

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

Di mode cerita, Tone Lock namanya **Style Lock**. Sebelum nulis bab pertama (atau pas ngelanjutin cerita orang), **tentuin dan catet** dulu kartu gaya ini. Kalau ceritanya udah ada, baca dulu bab-bab sebelumnya dan **tiru** pilihan yang udah dipakai — jangan diganti.

```yaml
# STYLE LOCK — isi sekali, pakai terus sampai tamat
judul: ""
genre: ""                # teenfic / romance / komedi / horor / thriller / fantasy / AU
rating: "13+"            # 13+ / 17+ / 21+ (ngaruh ke kata kasar)
pov: "orang pertama"     # orang pertama / orang ketiga terbatas / orang ketiga serba tahu / multi-POV
kata_ganti_narasi: "gue" # gue / aku / (nama tokoh, kalau POV 3)
kata_ganti_dialog: "gue-lo"  # gue-lo / aku-kamu / campur per karakter (tulis di voice sheet)
level_slang: 2           # 1 / 2 / 3 (lihat tabel level di SKILL.md)
ejaan_negasi: "nggak"    # nggak / gak / enggak — pilih SATU
code_mixing: "sedang"    # rendah / sedang / tinggi
italic_kata_asing: false # true = semua kata Inggris dimiringin; false = cuma yang jarang dipakai
latar: "Jakarta, 2026"
panjang_bab: "1.200-2.000 kata"
```

**Kalau user nggak ngasih info apa-apa**, pakai default ini:

| Setting | Default |
|---|---|
| POV | Orang pertama |
| Kata ganti | `gue-lo` (narasi dan dialog) |
| Level slang | 2 |
| Negasi | `nggak` |
| Code-mixing | Sedang |
| Rating | 13+ |
| Panjang bab | 1.200–2.000 kata |

### Kapan pakai gue-lo vs aku-kamu

| `gue-lo` | `aku-kamu` |
|---|---|
| Latar kota besar, tongkrongan, kampus, kantor startup | Cerita manis/soft, romance kalem, latar daerah, keluarga |
| Karakter ceplas-ceplos, sarkas, tengil | Karakter lembut, pendiam, sopan |
| Vibes komedi, chaos, banter | Vibes healing, melankolis, slice of life |

**Boleh campur**, tapi harus **ada alasannya** dan dicatet:
- Tokoh ngomong `gue-lo` ke temen, tapi `aku-kamu` ke pacar → ini *character development*, sah.
- Pergantian `gue-lo` → `aku-kamu` di tengah cerita = momen penting (misal jadian). Jadiin momen, jangan kebetulan.

---

## Aturan Khusus

### Narasi vs Dialog vs Batin vs Chat

Empat "bagian" ini punya aturan beda. Jangan ketuker.

| Bagian | Level slang | Singkatan | Partikel | Catatan |
|---|---|---|---|---|
| **Narasi** | Sesuai Style Lock | ❌ | Dikit | POV 1 lebih bebas; POV 3 lebih rapi |
| **Dialog** | Style Lock ± 1 sesuai karakter | ❌ | ✅ | Harus kedengeran kayak ngomong |
| **Batin** (italic) | Bisa paling liar | Jarang | ✅ | Tempat tokoh jujur dan nyeleneh |
| **Chat** | Level 3 boleh | ✅ | ✅ | Format khusus (lihat bagian Struktur dan Format) |

**POV 1 (gue/aku):** narasi = curhatan tokoh. Boleh nyeletuk, nyindir, ngomong ke pembaca.

> Gue benci hari Senin. Bukan benci biasa, tapi benci yang level *pengen pindah planet*.

**POV 3:** narasi lebih kalem, slang dikurangin satu level, tapi tetep pakai ejaan santai dan kalimat pendek. Celetukan tokoh disalurin lewat batin/dialog.

> Raka mendengus. Lagi-lagi Senin, lagi-lagi telat. *Kenapa sih Senin harus ada.*

### Voice Tiap Karakter

Biar tiap karakter kedengeran beda tapi tetap konsisten, bikin voice sheet sebelum nulis:

```yaml
- nama: Raka
  umur: 23
  kata_ganti: gue-lo (ke semua orang), aku-kamu (cuma ke ibunya)
  level_slang: 3
  code_mixing: tinggi ("literally", "which is")
  partikel_khas: "sih", "anjir"
  kata_kasar: "anjir", "sialan"
  kebiasaan_ngomong: sarkas, jawab pertanyaan pakai pertanyaan
  catchphrase: "Ya terus?"
  cara_chat: huruf kecil, nggak pernah pakai titik, spam stiker

- nama: Nadia
  umur: 22
  kata_ganti: aku-kamu
  level_slang: 1
  code_mixing: rendah
  partikel_khas: "kok", "ya"
  kata_kasar: nggak pernah, paling "ya ampun"
  kebiasaan_ngomong: kalem, kalimat lengkap, suka minta maaf
  catchphrase: "Nggak apa-apa, beneran."
  cara_chat: rapi, pakai huruf kapital, emoji 🙂
```

**Tes voice:** tutup nama di dialog. Kalau pembaca masih bisa nebak siapa yang ngomong = berhasil.

**Variasi daerah** (opsional, kalau latar mendukung):
- Rasa Jawa: *blas, wis, rek, cok* (rating!), *lho*, *to*.
- Rasa Sunda: *mah, teh, euy, atuh, -keun*.
- Rasa Betawi: *kagak, ente, aye, ngapa, kaga*.
- Rasa Medan: *kau, bah, cemana*.

Pakai **tipis-tipis** dan konsisten ke karakter itu aja.

### Hook (Kalimat Pembuka)

Kalimat pertama tiap bab harus bikin orang nggak bisa berhenti. Pilih salah satu:

| Jenis | Contoh |
|---|---|
| Pernyataan nyeleneh | "Kalau aja waktu itu gue nggak salah masuk toilet cowok, hidup gue nggak bakal se-chaos ini." |
| In media res (langsung di tengah aksi) | "Gue lari sekenceng-kencengnya sambil nenteng sebelah sepatu cowok yang barusan bikin gue hampir di-DO." |
| Dialog mengejutkan | "'Lo tau nggak, kita tuh sebenernya udah tunangan dari kecil?'" |
| Notif HP | "**1 pesan baru dari: Mantan 🚩**" |
| Pengakuan | "Oke, gue ngaku. Gue yang ngerusak motor Kak Dirga." |

❌ **Jangan buka pakai**: bangun tidur + liat jam, deskripsi cuaca, perkenalan diri ala biodata ("Namaku Rara, umurku 17 tahun, aku suka warna pink...").

### Cliffhanger (Penutup Bab)

Akhiri bab pas lagi tegang-tegangnya:
- Rahasia hampir kebongkar.
- Karakter tak terduga muncul.
- Pengakuan yang kepotong.
- Notif/telepon misterius.
- Satu kalimat pendek yang nonjok.

> Gue buka pintu, dan yang berdiri di situ bukan kurir.
>
> Itu dia. Cowok yang harusnya udah ada di Singapura.
>
> "Hai," katanya. "Kangen?"

### Show, Don't Tell

| Tell ❌ | Show ✅ |
|---|---|
| Rian marah banget. | Rian ngegebrak meja kantin sampai kuah baksonya tumpah. |
| Aku gugup. | Gue udah ngetik "hai" terus ngehapus lagi. Tujuh kali. |
| Dia cantik. | Satu kelas mendadak hening pas dia masuk. Bahkan Pak Darto lupa lanjutin absen. |

### Dialog yang Hidup

- **Kurangin dialog tag** ("katanya", "tanyanya", "ujarnya"). Ganti pakai **beat** (aksi kecil).

> ❌ "Kamu mau ke mana?" tanya Rara dengan penasaran. "Mau pergi," jawab Dirga dengan sinis.
>
> ✅ "Lo mau ke mana?" Rara berhenti di depan pintu.
>
> Dirga cuma ngelirik sekilas sambil masang helm. "Ke mana aja yang nggak ada lo."

- Kalau tag diperlukan, pakai yang simpel: **kata, tanya, bisik, teriak**. Jangan "ujarnya dengan nada penuh amarah yang membara".
- Orang nyata **motong omongan**, **nggak selesai ngomong**, **jawab nggak nyambung**. Pakai itu.
- Jangan ada dialog yang isinya cuma ngasih info ke pembaca ("Seperti yang kamu tahu, kita sudah sahabatan sejak SD dan ayahmu adalah CEO...").

### Paragraf dan Ritme

- 1–4 kalimat per paragraf. Kasih spasi lega (pembaca Wattpad baca di HP).
- Campur kalimat panjang dan pendek. Kalimat super pendek = efek dramatis.

> Dia pergi.
>
> Gitu aja. Tanpa pamit, tanpa chat, tanpa apa-apa.

- Satu kalimat satu paragraf boleh, tapi jangan tiap paragraf (jadi kayak puisi).

---

## Struktur dan Format

### Struktur Bab

| Bagian | Isi | Porsi |
|---|---|---|
| Hook | Kalimat/adegan pembuka yang narik | 5% |
| Bangun | Konflik kecil, interaksi, banter | 60% |
| Naik | Ketegangan/emosi meningkat | 25% |
| Cliffhanger | Gantung | 10% |

Panjang ideal: **1.200–2.000 kata**. Konsisten antarbab.

### Trope Wattpad yang Lagi Laku (2025–2026)

Pakai sebagai bahan, bukan rumus mati:
- **Enemies to lovers** — saling benci jadi saling suka.
- **Slow burn** — pelan-pelan, banyak tarik-ulur.
- **Forced proximity** — kepaksa bareng (satu kos, satu proyek, nikah kontrak).
- **Fake dating / nikah kontrak** — pura-pura pacaran.
- **Grumpy x sunshine** — si jutek ketemu si ceria.
- **Second chance** — balikan sama mantan.
- **AU lokal** — kampus, kantoran Jakarta, anak kos, AU idol/aktor.
- **Situationship / HTS drama** — relate banget sama pembaca 20-an.
- **Found family** — geng tongkrongan yang kayak keluarga.

### Author's Note (Opsional)

Kalau diminta nulis A/N, gayanya kayak ngobrol sama pembaca:

> **A/N:** Haii, maaf telat update 😭 minggu ini deadline kampus brutal banget. Btw kalian tim Raka atau tim Dirga? Spill di komen yaa. Jangan lupa vote biar aku semangat lanjutin! 💛

A/N **dipisah** dari isi cerita (pakai garis/judul A/N), jangan nyelip di tengah adegan.

### Tanda Baca dan Format

Bahasanya santai, tapi **tanda baca tetap rapi** (EYD tetap dihormati). Santai ≠ berantakan.

**Dialog:**
```
"Gue nggak peduli," kata Raka.          ← koma sebelum tag, tag huruf kecil
"Serius?" Nadia melotot.                 ← beat, huruf kapital (kalimat baru)
"Kalau lo pergi," katanya, "gue ikut."   ← dialog kepotong tag
"Tunggu—"                                ← omongan kepotong
"Aku... nggak tau."                      ← ragu
```

**Batin:** pakai *italic*, tanpa tanda kutip.
```
*Ya ampun, kenapa gue ngomong gitu sih.*
```

**Adegan chat** (pilih satu format, pakai terus):
```
**Raka**: udh sampe?
**Raka**: kok diread doang
**Nadia**: baru nyampe elah
**Nadia**: sabar napa 😭
```

**Pergantian adegan / POV:** pakai pemisah yang sama terus, misal `***` atau `— ✦ —`. Kalau multi-POV, kasih label: `**[ Raka ]**`.

**Tanda seru dan tanya:**
- Maksimal `?!` atau `!!` buat adegan heboh. Jangan `!!!!!!!`.
- Huruf kapital semua cuma buat teriak beneran, dan jarang.

**Emoji:** cuma di chat, sosmed, dan A/N. **Nggak boleh** di narasi dan dialog lisan.

**Angka:** satu sampai sembilan ditulis huruf di narasi ("tiga hari"), kecuali jam, tanggal, harga ("jam 2 pagi", "Rp25 ribu").

---

## Contoh

### Contoh 1 — Narasi POV 1

❌ **Kaku:**
> Pagi itu, aku terbangun dengan perasaan yang tidak menentu. Matahari bersinar dengan cerahnya, namun hatiku diselimuti oleh mendung yang kelabu. Aku sangat merindukan dirinya yang telah pergi meninggalkanku.

✅ **Santai (level 2):**
> Gue bangun jam sepuluh, dan hal pertama yang gue lakuin adalah ngecek HP.
>
> Nggak ada chat dari dia. Lagi.
>
> Gue lempar HP ke kasur, terus narik selimut sampai nutup muka. Di luar cerah banget, kayak semesta lagi ngeledek. *Iya, iya, cuma gue doang yang gamon di sini.*

### Contoh 2 — Dialog

❌ **Kaku:**
> "Apakah kamu sudah makan?" tanya Dimas.
>
> "Belum, aku tidak lapar," jawab Sinta.
>
> "Kamu harus makan agar tidak sakit," kata Dimas dengan perhatian.

✅ **Santai (level 2):**
> "Udah makan?"
>
> Sinta geleng, matanya masih nempel ke laptop. "Nggak laper."
>
> "Dari pagi lo bilang gitu." Dimas naruh sekotak martabak di sebelah laptopnya. "Makan. Gue tungguin sampe abis."
>
> "Lo bukan emak gue, Dim."
>
> "Ya makanya. Kalau emak lo yang dateng, lo udah diomelin dari tadi."

### Contoh 3 — Adegan Chat

> **Bima**: lo udh liat story nya kak arka blm\
> **Bima**: SUMPAH\
> **Bima**: dia upload foto sm cewe\
> **Lala**: hah\
> **Lala**: gmn\
> **Lala**: spill ss nya skrg jg\
> **Bima**: [foto]\
> **Lala**: anjir itu kan sepupunya 😭😭\
> **Lala**: lo delulu bgt sih bim\
> **Bima**: oh\
> **Bima**: oke gue hapus semua chat ini dan kita gapernah ngobrol

### Contoh 4 — Adegan Serius (slang diturunin)

> Ibu nggak bilang apa-apa waktu gue pulang. Cuma naruh teh anget di meja, terus duduk di sebelah gue.
>
> Lama. Cuma ada suara jam dinding.
>
> "Kalau capek," kata Ibu akhirnya, pelan banget, "pulang aja. Rumah ini nggak ke mana-mana."
>
> Dan di situ gue nangis. Nangis yang udah gue tahan dari bulan Maret.

Perhatiin: nggak ada slang tren, tapi tetap santai (*nggak, anget, gue, banget*). Itu yang dimaksud **konsisten tapi peka konteks**.

---

## Yang Dilarang

Selain anti-pattern umum di [SKILL.md](../SKILL.md#anti-pattern-umum), khusus cerita:

| ❌ Hindarin | ✅ Ganti jadi |
|---|---|
| "Di tengah hiruk-pikuk kota..." | Langsung ke adegan |
| "Seolah-olah dunia berhenti berputar" | "Otak gue nge-freeze." |
| "Jantungku berdegup kencang tak karuan" | "Jantung gue kayak abis lari keliling GBK." |
| "Perasaan yang tak terlukiskan dengan kata-kata" | Tunjukin lewat aksi |
| "Ia menghela napas panjang" (tiap 3 paragraf) | Variasi aksi lain |
| "Senyum tipis tersungging di bibirnya" | "Dia senyum dikit." |
| "Namun", "Akan tetapi", "Oleh karena itu" di dialog | "Tapi", "Makanya" |
| "Dirinya", "sang gadis", "pemuda itu" berulang | Pakai nama atau "dia" |
| "Tak", "kan", "jua" (puitis) | "Nggak", "bakal" |
| Penutup bab berupa kesimpulan/moral | Cliffhanger |

**Inkonsistensi (dosa paling besar):**
- ❌ Bab 1 `gue`, bab 3 tiba-tiba `aku` tanpa alasan.
- ❌ Satu paragraf ada `nggak`, `gak`, dan `tidak` sekaligus.
- ❌ Tokoh pendiem tiba-tiba ngomong kayak tukang roasting.
- ❌ Format chat bab 2 beda sama bab 5.
- ❌ Panggilan berubah-ubah ("Kak Dirga" → "Dirga" → "Bang Dirga") tanpa momen.

**Lain-lain:**
- ❌ Singkatan chat di narasi ("Gue udh capek bgt").
- ❌ Emoji di narasi.
- ❌ Infodump (deskripsi 3 paragraf soal wajah tokoh).
- ❌ Biodata di bab 1.
- ❌ Ngejelasin lelucon atau slang di dalam cerita ("Delulu, yang artinya delusional, adalah...").
- ❌ Slang dipakai salah arti (misal "gabut" buat "sibuk").
- ❌ Body shaming, rasis, atau slang peyoratif buat ngehina kelompok — kecuali buat nunjukin karakter itu jahat, dan ceritanya jelas nggak ngebenerin.

---

## Checklist

Jalanin ini tiap selesai nulis satu bab:

- [ ] Kata ganti narasi sama kayak Style Lock?
- [ ] Kata ganti tiap karakter sama kayak voice sheet?
- [ ] Ejaan negasi cuma satu versi (`nggak` / `gak` / `enggak`)?
- [ ] Nggak ada campuran `udah/sudah`, `aja/saja`, `kayak/seperti` di dialog?
- [ ] Level slang narasi sesuai Style Lock?
- [ ] Singkatan cuma muncul di adegan chat?
- [ ] Emoji cuma di chat/A/N?
- [ ] Italic kata asing konsisten?
- [ ] Format chat dan pemisah adegan sama kayak bab sebelumnya?
- [ ] Panggilan antar karakter konsisten?
- [ ] Bab dibuka pakai hook?
- [ ] Bab ditutup pakai cliffhanger / pertanyaan ngegantung?
- [ ] Paragraf maksimal 4 kalimat?
- [ ] Ada minimal satu momen show-don't-tell yang kuat?
- [ ] Nggak ada frasa "AI banget" dari tabel di atas?
- [ ] Adegan serius udah turunin slang?
- [ ] Kata kasar sesuai rating?
- [ ] Panjang bab di kisaran target?

---

## Format Output

**Kalau nulis bab:**
```markdown
# Bab [nomor]: [Judul Bab]

[isi cerita]

***

<!-- opsional, cuma kalau diminta -->
**A/N:** ...
```

Jangan kasih penjelasan, komentar, atau catatan di dalam isi cerita. Kalau perlu ngasih catatan ke user (misal "gue pakai default gue-lo karena nggak disebutin"), taruh **di luar** blok cerita, singkat aja.

**Kalau review:**
```markdown
## Hasil Review Konsistensi — Bab [nomor]

| Baris/kutipan | Masalah | Saran |
|---|---|---|
| "Aku tidak tau..." | Kata ganti dan negasi nggak sesuai Style Lock | "Gue nggak tau..." |
```

**Peran agent di mode cerita:**

| Peran | Tugas |
|---|---|
| **Penulis** | Nulis bab/adegan baru sesuai Style Lock. |
| **Editor gaya** | Ngubah tulisan kaku jadi santai tanpa ngubah plot. |
| **Reviewer konsistensi** | Nyari pelanggaran pakai checklist di atas, kasih daftar temuan + saran perbaikan per baris. |
| **Penulis chat scene** | Fokus ke aturan singkatan di [kamus-slang.md](../references/kamus-slang.md#3-singkatan-chat) dan format chat di atas. |
