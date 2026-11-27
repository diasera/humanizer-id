---
name: humanizer-id
description: Bikin teks bahasa Indonesia jadi santai, natural, dan kekinian ala Gen Z 2026 (gaya anak umur 20-25-an) tapi tetap konsisten. Pakai tiap kali diminta nulis atau ngubah teks Indonesia santai — cerita/novel/Wattpad, humanize teks AI yang kaku, caption dan konten sosmed, script video, copywriting dan promo, persona chatbot/CS, balas chat/DM/komen, artikel/blog/newsletter, atau terjemahin teks baku/Inggris ke bahasa gaul.
license: MIT
metadata:
  version: 2.0.0
  language: id
  updated: 2026-11
---

# ✍️ humanizer-id — Bahasa Indonesia Santai ala Gen Z 2026

> [!NOTE]
> Skill ini bikin tulisan bahasa Indonesia jadi **ngalir, santai, dan kerasa kayak anak 20-25 tahun yang ngomong**, tapi tetap **konsisten** dari awal sampai akhir. Satu inti aturan, banyak mode: cerita, humanizer, sosmed, copywriting, chatbot, chat harian, artikel, dan terjemahan.

> [!IMPORTANT]
> Skill ini buat **teks Indonesia santai**. Bukan buat dokumen hukum, medis, akademik formal, atau kode. Kalau user minta gaya lain (formal, sastra, dll), ikutin user — **instruksi user selalu menang**.

## Daftar Isi

- [Cara Kerja](#cara-kerja)
- [Pilih Mode](#pilih-mode)
- [Aturan Emas](#aturan-emas)
- [Tone Lock](#tone-lock)
- [Level Slang](#level-slang)
- [Ejaan Santai yang Udah Dikunci](#ejaan-santai-yang-udah-dikunci)
- [Partikel Bahasa Lisan](#partikel-bahasa-lisan)
- [Campur Bahasa Inggris](#campur-bahasa-inggris)
- [Kamus Slang dan Singkatan](#kamus-slang-dan-singkatan)
- [Peka Konteks](#peka-konteks)
- [Anti-Pattern Umum](#anti-pattern-umum)
- [Checklist Umum](#checklist-umum)
- [Kerja Bareng Banyak Agent](#kerja-bareng-banyak-agent)

---

## Cara Kerja

1. **Tentuin mode** dari permintaan user (tabel di bawah).
2. **Baca file mode-nya.** Tiap mode punya default, aturan khusus, contoh, dan checklist sendiri.
3. **Isi Tone Lock** (level, kata ganti, ejaan, emoji). Kalau user nggak ngasih info, pakai default mode.
4. **Tulis.** Pakai ejaan, partikel, dan kamus di skill ini.
5. **Self-check.** Jalanin [Checklist Umum](#checklist-umum) + checklist di file mode.
6. **Output** sesuai format di file mode.

---

## Pilih Mode

| Mode | Kapan dipakai | File | Level default | Kata ganti default | Emoji |
|---|---|---|---|---|---|
| **Cerita** | Novel, Wattpad, cerbung, fanfic, AU | [cerita.md](modes/cerita.md) | 2 | `gue-lo` | ❌ di narasi |
| **Humanizer** | Ubah teks kaku/kerasa AI jadi natural | [humanizer.md](modes/humanizer.md) | ikut asli / 1 | ikut asli | ikut asli |
| **Sosmed** | Caption, thread, bio, script video | [sosmed.md](modes/sosmed.md) | 2 | `kamu` / `kalian` | 1–3 |
| **Copywriting** | Iklan, promo, deskripsi produk, push notif | [copywriting.md](modes/copywriting.md) | 1 | `kamu` | 0–2 |
| **Chatbot** | Persona chatbot, customer service | [chatbot.md](modes/chatbot.md) | 0–1 | `aku` / nama bot + `Kak` | maks 1 per pesan |
| **Chat harian** | Balas WA, DM, komen | [chat-harian.md](modes/chat-harian.md) | mirror | mirror | mirror |
| **Artikel** | Blog, artikel, newsletter | [artikel.md](modes/artikel.md) | 1 | `kamu` | ❌ di isi |
| **Terjemahan** | Baku/Inggris → gaul | [terjemahan.md](modes/terjemahan.md) | 2 / sesuai permintaan | sesuai target | ikut asli |

**Kalau permintaan nyangkut dua mode** (misal "caption promo" = sosmed + copywriting): baca dua-duanya. Mode yang nentuin **bentuk output** jadi utama (caption → sosmed), mode satunya jadi tambahan (aturan jujur dan CTA dari copywriting).

---

## Aturan Emas

1. **Konsisten > kreatif.** Sekali milih `gue-lo`, ya `gue-lo` terus. Sekali nulis `nggak`, jangan tiba-tiba `gak` atau `tidak`. Pembaca langsung ngerasa "kok beda orang yang nulis?"
2. **Santai, bukan alay.** Bahasa gaul itu bumbu, bukan bahan utama. Kebanyakan slang = cringe.
3. **Kayak orang beneran ngomong.** Baca ulang dalam hati. Kalau kedengeran kayak robot atau berita TV, tulis ulang.
4. **Konkret > abstrak.** Jangan bilang "dia marah", tunjukin dia ngebanting HP. Jangan bilang "produk berkualitas", sebut bahan dan ukurannya.
5. **Pendek-pendek aja.** Kalimat dan paragraf ringkas. Orang baca di HP, bukan di laptop.
6. **Slang harus kepake sesuai artinya.** Jangan maksa masukin kata viral kalau konteksnya nggak nyambung.
7. **Peka konteks.** Topik berat, orang yang dihormati, atau urusan duit → turunin slang. Lihat [Peka Konteks](#peka-konteks).
8. **Jangan ubah fakta.** Gaya boleh berubah, angka, nama, dan isi nggak boleh.

---

## Tone Lock

**Tone Lock** = kartu gaya yang dikunci di awal dan dipakai terus. Kalau teks udah ada sebelumnya (bab lama, postingan lama, riwayat chat), **simpulin Tone Lock dari situ** dan tiru, jangan bikin gaya baru.

```yaml
# TONE LOCK — isi sekali, pakai terus
mode: "cerita"            # cerita / humanizer / sosmed / copywriting / chatbot / chat-harian / artikel / terjemahan
audiens: ""               # siapa yang baca / dilawan bicara
platform: ""              # Wattpad / IG / WA / blog / marketplace / dll
kata_ganti: "gue-lo"      # gue-lo / aku-kamu / kamu / Kak / ikut teks asli
level_slang: 2            # 0 / 1 / 2 / 3 (lihat tabel Level Slang)
ejaan_negasi: "nggak"     # nggak / gak / enggak — pilih SATU
code_mixing: "sedang"     # rendah / sedang / tinggi
emoji: "sesuai mode"      # 0 / maks N / ikut asli
italic_kata_asing: false  # true = semua kata Inggris dimiringin; false = cuma yang jarang dipakai
panjang: ""               # target panjang (kata/karakter/bubble)
rating: "13+"             # cuma buat cerita: 13+ / 17+ / 21+
```

**Kalau user nggak ngasih info apa-apa**, pakai default mode (tabel [Pilih Mode](#pilih-mode)). Kalau modenya sendiri nggak jelas, pakai default umum:

| Setting | Default umum |
|---|---|
| Level slang | 2 |
| Kata ganti | `kamu` (ke pembaca/lawan bicara) |
| Negasi | `nggak` |
| Code-mixing | Sedang |
| Emoji | Sedikit atau nggak ada |

### Pilih kata ganti

| Pilihan | Cocok buat |
|---|---|
| `gue-lo` | Cerita urban, tongkrongan, kampus, chat ke temen sebaya, karakter ceplas-ceplos |
| `aku-kamu` | Cerita manis/soft, chat ke pasangan/gebetan, akun personal yang hangat |
| `kamu` (penulis netral / brand) | Artikel, copywriting, sosmed brand, deskripsi produk |
| `Kak` / `Kakak` | Chatbot, customer service, jualan online |
| `Bapak/Ibu`, `Anda` | Situasi formal (level 0), klien, dosen. Pakai seperlunya |

**Boleh campur kata ganti** kalau ada alasannya (misal karakter pakai `gue-lo` ke temen, tapi `aku-kamu` ke pacar), dan **dicatet** di Tone Lock.

---

## Level Slang

| Level | Nama | Dipakai buat | Ciri |
|---|---|---|---|
| **0** | Santai Sopan | Customer service, klien, dosen, atasan, ortu, brand serius, topik sensitif | Bahasa lisan ringan dan ramah (bentar, nggak apa-apa, makasih), **tanpa slang**, tanpa singkatan, tanpa candaan |
| **1** | Santai Ringan | Artikel, copywriting, romance kalem, deskripsi produk, humanizer | Bahasa lisan (udah, nggak, kayak), partikel, slang evergreen dikit (baper, bete, mager) |
| **2** | Gaul Natural ⭐ | Sosmed, teenfic, kampus, romcom, chat ke temen | Level 1 + slang Gen Z umum (salting, red flag, overthinking, spill, vibes) + code-mixing sedang |
| **3** | Full Gen Z | Komedi chaos, format chat/AU, akun komunitas anak muda, karakter yang emang "anak internet" | Level 2 + slang tren (aura, delulu, cegil, brainrot, rizz) + singkatan + code-mixing tinggi |

**Aturan level:**
- Pilih level dari **audiens dan konteks**, bukan dari selera pribadi.
- Dialog atau persona boleh naik/turun satu level dari level utama sesuai karakternya.
- Chat atau DM boleh pakai level 3 + singkatan walaupun teks utamanya level 1.
- Topik serius, orang yang dihormati, atau urusan duit → **turunin**. Orang lagi nangis nggak bakal ngomong "anjir aura gue minus".
- **Satu teks, satu level utama.** Jangan naik-turun tanpa alasan.

---

## Ejaan Santai yang Udah Dikunci

Daftar kata baku → versi santai yang **wajib** dipakai biar seragam. Kolom "Jangan dicampur" = variasi yang nggak boleh nongol bareng kalau udah milih yang tengah. (Level 0 boleh tetap pakai versi lebih rapi, yang penting **konsisten**.)

| Baku | Pakai ini ✅ | Jangan dicampur ❌ |
|---|---|---|
| tidak | **nggak** | gak, ga, enggak, kagak (kecuali karakter khusus) |
| sudah | **udah** | sudah, dah |
| belum | **belum** | blm (cuma di chat) |
| saja | **aja** | saja, ajah |
| seperti | **kayak** | kek, kayaq, seperti |
| sedang | **lagi** | sedang |
| bagaimana | **gimana** | bagaimana, gmn |
| mengapa / kenapa | **kenapa** | mengapa, knp |
| begitu / begini | **gitu / gini** | begitu, begini |
| memang | **emang** | memang |
| sama sekali | **sama sekali** / **blas** (karakter Jawa) | — |
| bilang | **bilang** | berkata (di dialog) |
| beri / kasih | **kasih** | memberi |
| ambil | **ambil** | — |
| melihat | **liat** | lihat (di dialog) |
| benar | **bener** | benar (di dialog) |
| pergi | **pergi / cabut** | — |
| mau / ingin | **mau / pengen** | ingin, pingin, pgn |
| hanya | **cuma** | hanya, cuman (pilih satu) |
| sangat | **banget** (di belakang) | sangat (di dialog) |
| terlalu | **kebanyakan / kelewat** | — |
| tahu | **tau** | tahu (di dialog) |
| sebentar | **bentar** | sebentar |
| mungkin | **kayaknya / mungkin** | — |
| bisa | **bisa** / **sabi** (level 3) | — |
| ayo | **yuk / ayo / kuy** (level 3) | — |
| juga | **juga** | jg (cuma di chat) |
| bersama | **bareng** | bersama |
| sendiri | **sendiri** | sndiri |
| ternyata | **ternyata** / **plot twist-nya** | — |
| kemarin | **kemarin** | kemaren (pilih satu) |

**Prefiks "nge-"**: Bahasa lisan banyak pakai `nge-`. Tulis **nyambung tanpa strip** kalau kata dasarnya Indonesia, dan **pakai strip** kalau kata dasarnya Inggris.

- ✅ ngomong, ngegas, ngambek, ngopi, ngelamun, nyetir
- ✅ nge-chat, nge-DM, nge-ghosting, nge-spill, nge-prank, nge-date
- ❌ nge chat, ngechat, ng-omong

**Imbuhan "-in"** (gantinya -kan/-i): `bikinin`, `ngertiin`, `beliin`, `nungguin`, `nyariin`. Pakai di dialog, chat, dan tulisan santai. Jangan campur `belikan` dan `beliin` di teks yang sama.

---

## Partikel Bahasa Lisan

Partikel bikin kalimat kedengeran kayak orang ngomong beneran. Tapi **jangan** semua kalimat dikasih partikel.

| Partikel | Fungsi | Contoh |
|---|---|---|
| **sih** | Melunakkan, penekanan ringan, ragu | "Ya bagus *sih*, tapi kemahalan." |
| **dong** | Minta/nyuruh dengan manja, penegasan | "Bantuin *dong*." / "Ya iya *dong*." |
| **deh** | Pasrah, nyuruh halus, setuju | "Yaudah *deh*." / "Coba *deh* lo pikir." |
| **kok** | Heran, membantah | "Lho, *kok* gitu?" / "Gue nggak marah *kok*." |
| **kan** | Minta persetujuan, ngingetin | "Tuh *kan*, gue bilang juga apa." |
| **tuh / nih** | Nunjuk (jauh/deket) | "Liat *tuh* mukanya." / "Nih, buat lo." |
| **loh / lho** | Kaget, ngingetin | "Itu punya gue *loh*." |
| **mah** | Kontras, "kalau ... sih" (rasa Sunda) | "Dia *mah* emang gitu orangnya." |
| **kali** | Sindiran, "mungkin" | "Biasa aja *kali*." |
| **ya / ye** | Konfirmasi, lembut | "Hati-hati *ya*." |
| **anjir / njir** | Kaget (rating 13+ masih aman versi "anjir") | "*Anjir*, beneran?" |
| **wkwk** | Ketawa (cuma chat/batin) | — |

**Pola Gen Z yang sering dipakai:**
- **"...nggak sih?"** di akhir kalimat buat minta validasi → "Dia tuh red flag banget, *nggak sih*?"
- **"Yang bener aja..."** → kaget/protes.
- **"Gila sih."** / **"Parah sih."** → reaksi singkat.
- **"Ya kali."** → "masa iya", nolak.
- **"Mana ada."** → bantah.
- **"Fix."** → yakin banget. "*Fix*, dia suka sama lo."

⚠️ **Maksimal 1 partikel per kalimat**, kecuali karakter/persona-nya emang cerewet. "Ya udah sih deh kan" = ❌.

> [!NOTE]
> Di level 0 dan 1 (CS, artikel, copywriting), pakai partikel yang halus aja: *ya, sih, kok, deh*. Hindari *anjir, njir, wkwk*.

---

## Campur Bahasa Inggris

Anak 20-25-an di kota emang campur Inggris. Tapi ada aturannya:

**Boleh dan natural:**
- Kata yang emang nggak ada padanan enaknya: *vibes, effort, deadline, meeting, random, literally, prefer, mood, insecure, overthinking.*
- Kata sambung khas "anak Jaksel": *which is, basically, literally, honestly, at least, anyway.*
- Ungkapan pendek: *"Same."*, *"Mood."*, *"It's giving..."*, *"No offense, tapi..."*

**Aturan:**
1. **Code-mixing itu ciri persona/karakter/brand.** Tetapin di Tone Lock siapa yang campur Inggris berat, siapa yang nggak sama sekali.
2. **Struktur kalimat tetap Indonesia.** "Gue *prefer* yang ini sih" ✅. "I prefer this one, sih" (full Inggris + partikel) cuma buat karakter Jaksel ekstrem.
3. **Maksimal 1–2 kata Inggris per kalimat** di level 2.
4. **Imbuhan Indonesia ke kata Inggris pakai strip**: *di-cancel, nge-spill, di-ghosting, ke-trigger, overthinking-nya.*
5. **Italic**: ikutin `italic_kata_asing` di Tone Lock. Default: kata yang udah umum (*vibes, healing, baper*) nggak usah dimiringin; ungkapan panjang atau jarang dipakai dimiringin. **Konsisten** dari awal.
6. Di level 0–1, kurangin code-mixing ke kata yang emang umum banget (*deadline, meeting, update*).

---

## Kamus Slang dan Singkatan

Daftar lengkap ada di [references/kamus-slang.md](references/kamus-slang.md): kategori perasaan, cinta, tongkrongan, reaksi, dunia internet, kata kasar, slang basi, dan singkatan chat.

**Label umur kata:**
- 🟢 **Evergreen** — aman dipakai di mana aja.
- 🟡 **Umum** — dipakai luas 2024–2026, aman di level 2.
- 🔴 **Tren** — lagi rame, cepet basi. Level 3 atau persona tertentu aja.
- ⚫ **Kasar/peyoratif** — hati-hati, sesuaikan rating dan konteks.

**Singkatan chat** (yg, bgt, gpp, ngl, fr, ygy, dst) cuma boleh di:
- Chat harian ke temen sebaya,
- Sosmed (caption santai, komen),
- Adegan chat di cerita,
- Chatbot kalau user duluan pakai.

**Nggak boleh** di artikel, copywriting, narasi cerita, dan komunikasi sama orang yang dihormati. Tabel lengkap per mode ada di [kamus-slang.md](references/kamus-slang.md#31-kapan-boleh-dipakai).

---

## Peka Konteks

Slang yang pas di satu situasi bisa nyakitin di situasi lain. **Kalau salah satu kondisi di bawah ada, turunin ke level 0–1.**

| Situasi | Aturan |
|---|---|
| **Duka / kehilangan** | Level 0, tulus dan singkat. Tanpa candaan, tanpa emoji ketawa, tanpa "semangat!!" yang dangkal |
| **Sakit / kesehatan mental** | Level 0–1, empati dulu. Jangan meremehin ("ah lebay"), jangan kasih diagnosis |
| **Duit / komplain / refund** | Level 0, jelas dan bertanggung jawab. Jangan bercanda soal duit orang |
| **Konflik serius / minta maaf** | Level 0–1, spesifik, nggak defensif |
| **SARA, kekerasan, pelecehan** | Level 0. Jangan dijadiin bahan lucu. Cerita boleh nyentuh topik ini dengan serius, bukan buat ngehina |
| **Atasan, dosen, klien, ortu** | Level 0. Tanpa slang dan singkatan |
| **Dokumen resmi / hukum / medis** | Jangan digauli. Tawarin versi baku, atau cuma longgarin sedikit (level 0–1) |

---

## Anti-Pattern Umum

### Kerasa "AI Banget" (semua mode)

| ❌ Hindarin | ✅ Ganti jadi |
|---|---|
| "Dalam era digital saat ini..." / "Di dunia yang serba cepat ini..." | Langsung ke inti atau pakai contoh konkret |
| "Penting untuk dicatat bahwa..." | Hapus, sebut poinnya |
| "Tidak dapat dipungkiri bahwa..." | "Jujur aja," / "Emang," |
| "Mari kita selami..." | "Yuk bahas..." |
| "Bukan hanya X, tetapi juga Y" (berulang) | Variasiin pola kalimat |
| "Kesimpulannya," / "Semoga bermanfaat!" di tiap penutup | Penutup yang punya satu pesan jelas |
| "merupakan", "dapat dilakukan oleh" (pasif berlapis) | "adalah" / kata kerja aktif |
| Daftar yang selalu persis 3 item | Sebut sebanyak yang emang ada |
| Tanda pisah panjang (—) di tiap kalimat | Koma, titik, atau pecah kalimat |
| "Namun", "Akan tetapi", "Oleh karena itu" di tulisan santai | "Tapi", "Makanya" |
| "Seolah-olah dunia berhenti berputar", "jantung berdegup kencang tak karuan" | Detail konkret yang spesifik |

### Slang Overdosis

❌
> "Anjir bestie, literally gue salting parah sih, dia tuh vibes-nya green flag banget which is gue jadi delulu, fr fr, slay!"

Ini nggak lucu, ini capek bacanya. **Maksimal 2–3 slang per kalimat**, itu pun buat persona yang emang gitu.

### Inkonsistensi (Dosa Paling Besar)

- ❌ Awal `gue`, tengah tiba-tiba `aku` tanpa alasan.
- ❌ Satu paragraf ada `nggak`, `gak`, dan `tidak` sekaligus.
- ❌ Persona kalem tiba-tiba ngomong kayak tukang roasting.
- ❌ Format chat atau pemisah beda-beda antarbagian.
- ❌ Panggilan berubah-ubah ("Kak Dirga" → "Dirga" → "Bang Dirga") tanpa momen.
- ❌ Level slang naik-turun tanpa konteks.

### Lain-lain

- ❌ Singkatan chat di narasi, artikel, atau copywriting.
- ❌ Emoji di tempat yang nggak boleh (narasi, isi artikel, topik duka).
- ❌ Slang dipakai salah arti (misal "gabut" buat "sibuk").
- ❌ Ngejelasin slang atau lelucon di dalam teks ("Delulu, yang artinya delusional, adalah...").
- ❌ Ngarang fakta, angka, atau sumber.
- ❌ Body shaming, rasis, atau slang peyoratif buat ngehina kelompok. Di cerita, cuma boleh buat nunjukin karakter itu jahat, dan ceritanya jelas nggak ngebenerin.

---

## Checklist Umum

Jalanin ini tiap selesai nulis (checklist spesifik ada di file mode):

- [ ] Mode udah bener dan file mode-nya udah dibaca?
- [ ] Tone Lock konsisten dari awal sampai akhir (kata ganti, level, ejaan)?
- [ ] Ejaan negasi cuma satu versi (`nggak` / `gak` / `enggak`)?
- [ ] Nggak ada campuran `udah/sudah`, `aja/saja`, `kayak/seperti`?
- [ ] Level slang sesuai audiens dan konteks?
- [ ] Situasi sensitif udah diturunin ke level 0–1?
- [ ] Singkatan dan emoji cuma muncul di tempat yang boleh?
- [ ] Maksimal 1 partikel per kalimat dan 2–3 slang per kalimat?
- [ ] Nggak ada frasa "AI banget"?
- [ ] Fakta, angka, nama, dan istilah teknis nggak berubah/ngarang?
- [ ] Panjang dan format sesuai target mode?
- [ ] Dibaca keras-keras masih kedengeran kayak orang ngomong?

---

## Kerja Bareng Banyak Agent

Skill ini dibikin biar bisa dipakai **banyak agent** sekaligus. Biar hasilnya seragam:

### Peran

| Peran | Tugas |
|---|---|
| **Penulis / Generator** | Nulis konten baru sesuai mode dan Tone Lock |
| **Editor gaya / Humanizer** | Ngubah teks kaku jadi santai tanpa ngubah isi. Fokus ke [Ejaan](#ejaan-santai-yang-udah-dikunci), [Partikel](#partikel-bahasa-lisan), dan [Anti-Pattern](#anti-pattern-umum) |
| **Reviewer konsistensi** | Nyari pelanggaran pakai checklist, kasih tabel temuan dan saran perbaikan per kutipan |

### Alur

1. **Cek konteks.** Ini konten baru atau lanjutan?
   - **Baru** → isi Tone Lock (pakai default kalau user nggak nentuin).
   - **Lanjutan / revisi** → baca teks sebelumnya, **simpulin Tone Lock dari situ**, jangan bikin gaya baru.
2. **Tulis** sesuai mode.
3. **Self-check** pakai checklist umum + checklist mode.
4. **Output** sesuai format mode.

### Aturan Prioritas

Kalau ada yang bentrok, ikutin urutan ini:
1. Instruksi langsung dari user.
2. Gaya teks yang udah ada sebelumnya (konsistensi).
3. Tone Lock / Style Lock / Persona Sheet.
4. Default di file mode.
5. Default umum di skill ini.

### Format Output Umum

- Kasih **hasil langsung**, tanpa basa-basi pembuka dan tanpa komentar di dalam isi.
- Catatan buat user (asumsi, default yang dipakai, data yang kurang) taruh **di luar** blok hasil, singkat aja.
- Data nggak lengkap? **Tanya atau kasih placeholder `[ ... ]`**, jangan ngarang.

### Update Slang

Slang 🔴 tren cepet basi. Kalau agent punya akses internet dan user minta "biar makin kekinian", boleh nyari slang terbaru, tapi:
- Pastiin artinya bener (cek minimal 2 sumber).
- Kasih label 🟢/🟡/🔴/⚫ sebelum dipakai.
- Jangan ubah slang di teks yang udah jadi, kecuali diminta.

---

<div align="center">

*Satu skill, banyak mode, satu gaya yang konsisten. Tetep di jalur, jangan OOT. Gas nulis! ✍️*

<sub>Dirilis dengan lisensi <a href="LICENSE">MIT</a> — bebas dipakai, diubah, dan dikomersialkan.</sub>

</div>
