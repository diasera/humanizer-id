---
name: humanizer-id
description: Panduan gaya bahasa buat nulis cerita Wattpad / novel pakai bahasa Indonesia modern 2026 yang santai, nggak kaku, penuh slang dan singkatan Gen Z, tapi tetap konsisten dari bab pertama sampai tamat. Pakai skill ini tiap kali diminta nulis, ngelanjutin, ngedit, atau nge-review cerita fiksi (bab, prolog, dialog, chat scene, blurb, author's note) dengan gaya anak muda umur 20-25-an.
license: MIT
metadata:
  version: 1.0.0
  language: id
  updated: 2026-11
---

# ✍️ humanizer-id — Gaya Bahasa Wattpad & Novel Gen Z 2026

> [!NOTE]
> Skill ini khusus buat **nulis cerita fiksi** (Wattpad, novel online, cerbung, AU, fanfic). Fokusnya satu: bikin tulisan yang **ngalir, santai, kerasa kayak anak 20-25 tahun yang ngomong**, dan **konsisten** dari awal sampai akhir.

> [!IMPORTANT]
> Jangan dipakai buat nulis dokumen resmi, kode, email kantor, atau hal lain di luar cerita. Kalau user minta gaya lain (misal formal/sastra), ikutin user — instruksi user selalu menang.

---

## Daftar Isi

1. [Aturan Emas (Wajib Banget)](#1-aturan-emas-wajib-banget)
2. [Kunci Gaya Dulu Sebelum Nulis (Style Lock)](#2-kunci-gaya-dulu-sebelum-nulis-style-lock)
3. [Level Slang](#3-level-slang)
4. [Ejaan Santai yang Udah Dikunci](#4-ejaan-santai-yang-udah-dikunci)
5. [Partikel: Nyawanya Bahasa Lisan](#5-partikel-nyawanya-bahasa-lisan)
6. [Kamus Slang Gen Z 2026](#6-kamus-slang-gen-z-2026)
7. [Singkatan Chat](#7-singkatan-chat)
8. [Campur Bahasa Inggris (Code-Mixing)](#8-campur-bahasa-inggris-code-mixing)
9. [Narasi vs Dialog vs Batin vs Chat](#9-narasi-vs-dialog-vs-batin-vs-chat)
10. [Teknik Nulis ala Wattpad](#10-teknik-nulis-ala-wattpad)
11. [Format & Tanda Baca](#11-format--tanda-baca)
12. [Voice Tiap Karakter](#12-voice-tiap-karakter)
13. [Contoh Kaku vs Santai](#13-contoh-kaku-vs-santai)
14. [Yang Haram Dilakuin (Anti-Pattern)](#14-yang-haram-dilakuin-anti-pattern)
15. [Checklist Konsistensi](#15-checklist-konsistensi)
16. [Cara Agent Pakai Skill Ini](#16-cara-agent-pakai-skill-ini)

---

## 1. Aturan Emas (Wajib Banget)

1. **Konsisten > kreatif.** Sekali milih `gue-lo`, ya `gue-lo` terus. Sekali nulis `nggak`, jangan tiba-tiba `gak` atau `ga`. Pembaca langsung ngerasa "kok beda orang yang nulis?"
2. **Santai, bukan alay.** Bahasa gaul itu bumbu, bukan bahan utama. Kebanyakan slang = cringe.
3. **Kayak orang beneran ngomong.** Baca ulang dialognya dalam hati. Kalau kedengeran kayak robot atau berita TV, tulis ulang.
4. **Narasi boleh rapi, dialog harus hidup.** Narasi tetep santai, tapi nggak sepadat dialog soal slang.
5. **Show, don't tell.** Jangan bilang "dia marah", tunjukin dia ngebanting HP ke kasur.
6. **Pendek-pendek aja.** Paragraf 1-4 kalimat. Pembaca Wattpad baca di HP, bukan di laptop.
7. **Tiap bab harus bikin penasaran.** Buka pakai hook, tutup pakai cliffhanger atau minimal pertanyaan yang ngegantung.
8. **Slang harus kepake sesuai artinya.** Jangan maksa masukin kata viral kalau konteksnya nggak nyambung.

---

## 2. Kunci Gaya Dulu Sebelum Nulis (Style Lock)

Sebelum nulis bab pertama (atau pas ngelanjutin cerita orang), **tentuin dan catet** dulu kartu gaya ini. Kalau ceritanya udah ada, baca dulu bab-bab sebelumnya dan **tiru** pilihan yang udah dipakai — jangan diganti.

```yaml
# STYLE LOCK — isi sekali, pakai terus sampai tamat
judul: ""
genre: ""                # teenfic / romance / komedi / horor / thriller / fantasy / AU
rating: "13+"            # 13+ / 17+ / 21+ (ngaruh ke kata kasar)
pov: "orang pertama"     # orang pertama / orang ketiga terbatas / orang ketiga serba tahu / multi-POV
kata_ganti_narasi: "gue" # gue / aku / (nama tokoh, kalau POV 3)
kata_ganti_dialog: "gue-lo"  # gue-lo / aku-kamu / campur per karakter (tulis di voice sheet)
level_slang: 2           # 1 / 2 / 3 (lihat bagian 3)
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
| Kata ganti | `gue-lo` (narasi & dialog) |
| Level slang | 2 |
| Negasi | `nggak` |
| Code-mixing | Sedang |
| Rating | 13+ |
| Panjang bab | 1.200–2.000 kata |

### Kapan pakai `gue-lo` vs `aku-kamu`?

| `gue-lo` | `aku-kamu` |
|---|---|
| Latar kota besar, tongkrongan, kampus, kantor startup | Cerita manis/soft, romance kalem, latar daerah, keluarga |
| Karakter ceplas-ceplos, sarkas, tengil | Karakter lembut, pendiam, sopan |
| Vibes komedi, chaos, banter | Vibes healing, melankolis, slice of life |

**Boleh campur**, tapi harus **ada alasannya** dan dicatet:
- Tokoh ngomong `gue-lo` ke temen, tapi `aku-kamu` ke pacar → ini *character development*, sah.
- Pergantian `gue-lo` → `aku-kamu` di tengah cerita = momen penting (misal jadian). Jadiin momen, jangan kebetulan.

---

## 3. Level Slang

| Level | Nama | Dipakai buat | Ciri |
|---|---|---|---|
| **1** | Santai Ringan | Romance kalem, drama keluarga, novel cetak | Bahasa lisan (udah, nggak, kayak), partikel, slang evergreen dikit (baper, bete, mager) |
| **2** | Gaul Natural ⭐ | Teenfic, kampus, romcom, kebanyakan cerita Wattpad | Level 1 + slang Gen Z umum (salting, red flag, overthinking, spill, vibes) + code-mixing sedang |
| **3** | Full Gen Z | Komedi chaos, cerita format chat/AU, karakter yang emang "anak internet" | Level 2 + slang tren (aura, delulu, cegil, brainrot, rizz) + singkatan + code-mixing tinggi |

**Aturan level:**
- Level berlaku buat **narasi**. Dialog boleh naik satu level tergantung karakternya.
- Adegan chat/DM boleh pakai level 3 + singkatan walaupun cerita aslinya level 1.
- Adegan sedih/serius → **turunin** slang. Orang lagi nangis nggak bakal ngomong "anjir aura gue minus".

---

## 4. Ejaan Santai yang Udah Dikunci

Ini daftar kata baku → versi santai yang **wajib** dipakai biar seragam. Kolom "Jangan" = variasi yang nggak boleh dicampur kalau udah milih yang kiri.

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

**Imbuhan "-in"** (gantinya -kan/-i): `bikinin`, `ngertiin`, `beliin`, `nungguin`, `nyariin`. Pakai di dialog dan narasi santai. Jangan campur `belikan` dan `beliin` di cerita yang sama.

---

## 5. Partikel: Nyawanya Bahasa Lisan

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

⚠️ **Maksimal 1 partikel per kalimat**, kecuali karakternya emang cerewet. "Ya udah sih deh kan" = ❌.

---

## 6. Kamus Slang Gen Z 2026

Label umur kata:
- 🟢 **Evergreen** — aman dipakai di narasi, nggak bakal basi.
- 🟡 **Umum** — dipakai luas 2024–2026, aman di dialog & narasi level 2.
- 🔴 **Tren** — lagi rame, cepet basi. Pakai di dialog karakter tertentu aja, level 3.
- ⚫ **Kasar/peyoratif** — hati-hati, sesuaiin rating & karakter.

### 6.1 Perasaan & Mental

| Kata | Arti | Label | Contoh |
|---|---|---|---|
| baper | bawa perasaan | 🟢 | "Jangan baper, dia emang ramah ke semua orang." |
| bete / badmood | kesel, mood jelek | 🟢 | "Gue lagi bete, jangan ganggu." |
| mager | males gerak | 🟢 | "Mager banget mau mandi." |
| gabut | gaji buta → nggak ada kerjaan, bosen | 🟢 | "Gabut, akhirnya gue scroll TikTok sampe subuh." |
| salting | salah tingkah | 🟡 | "Dia senyum dikit, gue langsung salting." |
| overthinking | mikir kebanyakan | 🟡 | "Udah jam dua pagi dan gue masih overthinking." |
| insecure | nggak pede | 🟡 | "Liat feed dia, gue auto insecure." |
| galau | bingung + sedih | 🟢 | — |
| healing | liburan / nyegerin diri | 🟡 | "Butuh healing ke Bandung, minimal." |
| burnout | capek mental parah | 🟡 | — |
| quarter life crisis | krisis umur 20-an | 🟡 | "Umur 24 dan gue resmi masuk era quarter life crisis." |
| mental breakdown | mental ambruk | 🟡 | — |
| salty | sewot, kesel, iri | 🟡 | "Kok lo salty gitu sih?" |
| FOMO | takut ketinggalan | 🟡 | — |
| JOMO | seneng nggak ikut-ikutan | 🔴 | "Malam minggu di kamar? JOMO, bukan jomblo." |
| TBL | takut banget loh | 🔴 | "TBL, sumpah." |
| IBL / SBL | iri / sebel banget loh | 🔴 | — |
| ilfeel / ick | ilang feeling | 🟡 | "Dia ngunyah sambil mangap. Ilfeel, langsung kena ick." |
| receh | humornya gampang ketawa | 🟢 | "Selera humor gue receh banget." |
| gemes / gemoy | lucu bikin pengen nyubit | 🟢 | — |
| kepo | pengen tau urusan orang | 🟢 | — |
| nangis kejer | nangis parah | 🟢 | — |

### 6.2 Cinta & Hubungan

| Kata | Arti | Label | Contoh |
|---|---|---|---|
| bucin | budak cinta | 🟢 | "Sejak jadian, dia bucin akut." |
| PDKT | pendekatan | 🟢 | — |
| HTS | hubungan tanpa status | 🟡 | "Tiga bulan HTS, ujungnya dia jadian sama orang lain." |
| situationship | hubungan nggak jelas | 🟡 | — |
| red flag / green flag | tanda bahaya / tanda baik | 🟡 | "Cemburu sama kucing gue? Red flag." |
| ghosting | ngilang tanpa kabar | 🟡 | "Udah seminggu dia ghosting gue." |
| gaslighting | manipulasi bikin ngerasa salah | 🟡 | — |
| love bombing | banjirin perhatian di awal | 🟡 | — |
| friendzone | dianggap temen doang | 🟢 | — |
| gamon | gagal move on | 🟡 | "Udah setahun, masih gamon." |
| delulu | delusional, halu soal cinta | 🔴 | "Dia bales 'oke' doang dan gue udah mikirin nama anak. Delulu." |
| halu | halusinasi, ngayal | 🟢 | — |
| cegil / cogil | cewek gila / cowok gila (bucin ekstrem, unpredictable) | 🔴 | "Gue nge-stalk mantannya sampe 2019. Cegil era." |
| pick me | caper biar dianggap beda | 🔴 | "Aku mah beda, nggak suka dandan." — *pick me banget.* |
| rizz | skill ngegombal/ngerayu | 🔴 | "Rizz-nya nol, tapi mukanya bikin maafin." |
| ngedate | kencan | 🟡 | — |
| uwu | gemes romantis | 🟡 | — |
| ayang | sayang (manja) | 🟡 | — |
| mokondo | cowok yang cuma numpang/manfaatin pasangan | ⚫ | Kasar. Cuma buat karakter yang emang julid, rating 17+. |

### 6.3 Tongkrongan & Pertemanan

| Kata | Arti | Label | Contoh |
|---|---|---|---|
| bestie | sahabat | 🟡 | — |
| bro / bang / ngab | panggilan cowok (ngab = bang dibalik) | 🟡 | "Santai, ngab." |
| cuy / coy | panggilan santai | 🟢 | — |
| nongki | nongkrong | 🟢 | — |
| circle | geng | 🟡 | "Circle gue isinya orang gabut semua." |
| mutualan | saling follow | 🟡 | — |
| julid | nyinyir | 🟢 | — |
| nolep | no life, jarang keluar | 🟡 | — |
| anak skena | anak gaul gigs/kopi/thrift | 🔴 | — |
| kalcer | culture, gaya hidup "keren" | 🔴 | — |
| orang have / orang clear | orang kaya / orang lagi bokek | 🔴 | "Gue lagi jadi orang clear, tanggal tua." |
| bokek | nggak ada duit | 🟢 | — |
| tanggal tua | akhir bulan, dompet tipis | 🟢 | — |
| nebeng | numpang | 🟢 | — |
| gercep | gerak cepat | 🟡 | — |
| japri | jalur pribadi (chat pribadi) | 🟢 | — |
| gaje | nggak jelas | 🟢 | — |

### 6.4 Reaksi & Penilaian

| Kata | Arti | Label | Contoh |
|---|---|---|---|
| anjir / anjay / bjir | kaget/kagum | 🟡 | — |
| gila sih / parah | kagum/kaget | 🟢 | — |
| kocak | lucu, absurd | 🟢 | — |
| cringe | bikin malu sendiri | 🟡 | — |
| valid | bener, masuk akal | 🟡 | "Perasaan lo valid kok." |
| relate | ngerasain hal yang sama | 🟡 | — |
| real / fr | beneran, setuju | 🔴 | "Real sih." |
| no debat | nggak usah dibantah | 🟡 | — |
| slay | keren maksimal | 🔴 | — |
| aura / +1000 aura / minus aura | karisma naik / malu-maluin | 🔴 | "Kepeleset di depan gebetan. Minus seribu aura." |
| aura farming | sengaja pasang gaya biar keren | 🔴 | — |
| sus | mencurigakan | 🔴 | — |
| random | acak, nggak nyambung | 🟢 | — |
| plot twist | kejadian tak terduga | 🟢 | — |
| main character energy | ngerasa jadi tokoh utama | 🔴 | — |
| NPC | orang yang datar/ikut-ikutan | 🔴 | — |
| mantul | mantap betul | 🟡 | — |
| sabi | bisa (dibalik) | 🟡 | — |
| gaskeun / gas | ayo langsung | 🟡 | — |
| skip | lewatin, nolak | 🟢 | — |
| effort | usaha | 🟡 | "Effort-nya keliatan, sih." |
| spill | bocorin, ceritain | 🟡 | "Spill dong siapa orangnya." |
| clock it | ngebongkar fakta telak | 🔴 | — |

### 6.5 Dunia Internet

| Kata | Arti | Label |
|---|---|---|
| FYP | For You Page, viral | 🟡 |
| ngonten | bikin konten | 🟡 |
| brainrot | otak "rusak" kebanyakan konten absurd | 🔴 |
| doomscrolling | scroll tanpa henti | 🟡 |
| stalk / kepoin | ngintip akun orang | 🟢 |
| close friend (CF) | story khusus temen deket | 🟡 |
| PAP | post a picture, kirim foto | 🟡 |
| war tiket | rebutan tiket konser | 🟡 |
| ratio / ke-ratio | dikomen lebih banyak dari postingannya | 🔴 |
| pansos | panjat sosial | 🟢 |

### 6.6 Kata Kasar (Atur Sesuai Rating)

| Rating | Boleh |
|---|---|
| 13+ | anjir, sialan, brengsek (jarang), astaga, ya ampun |
| 17+ | + bangsat, tai, goblok (tokoh tertentu aja) |
| 21+ | Sesuai kebutuhan cerita, tapi tetap nggak tiap kalimat |

Kata kasar = **ciri karakter**, bukan ciri penulis. Tokoh sopan nggak tiba-tiba misuh.

> 🗑️ **Slang basi yang dilarang** (kecuali buat ngelawak/karakter jadul): ciyus, miapah, cemungudh, kamseupay, sesuatu banget, 4l4y (huruf-angka), w0w, eaaa, baper-baperan alay ala 2012, "unch".

---

## 7. Singkatan Chat

Singkatan **cuma boleh** dipakai di:
1. Adegan chat/DM/WA/komen sosmed,
2. Tulisan di HP yang dibaca tokoh,
3. Batin tokoh yang emang chronically online (level 3, jarang-jarang).

**Nggak boleh** dipakai di narasi biasa atau dialog lisan (orang nggak ngomong "yg" atau "bgt" pakai mulut).

| Singkatan | Kepanjangan |
|---|---|
| yg | yang |
| bgt | banget |
| gpp / gapapa | nggak apa-apa |
| udh / dh | udah |
| blm | belum |
| sm | sama |
| gmn | gimana |
| knp | kenapa |
| kpn | kapan |
| dmn | di mana |
| otw | on the way (sering padahal belum mandi) |
| btw | by the way |
| ywdh / yaudh | yaudah |
| gws | get well soon |
| tbh | to be honest |
| idk | i don't know |
| ngl | not gonna lie |
| fr | for real |
| imo | in my opinion |
| ygy | ya guys ya |
| cmiiw | correct me if i'm wrong |
| nt | nice try |
| jir / njir | anjir |
| wkwk / wkwkwk | ketawa |
| awokwok | ketawa ngeledek |
| hehe | ketawa canggung |
| WKWKWK (caps) | ketawa ngakak beneran |
| 😭 | bukan sedih, tapi ngakak/gemes (Gen Z banget) |
| 💀 | "mati ketawa" / malu parah |

**Gaya ketik chat Gen Z 2026:**
- Huruf kecil semua, jarang titik di akhir. Titik di akhir chat = kesannya marah/dingin. ("oke." vs "okee")
- Huruf diulang buat nada: "iyaaa", "plisss", "hah??"
- Bubble pendek-pendek, dikirim beruntun.
- Pakai "sksksk", "AAAAA", "HAH" kalau panik/gemes.

---

## 8. Campur Bahasa Inggris (Code-Mixing)

Anak 20-25-an di kota emang campur Inggris. Tapi ada aturannya:

**Boleh dan natural:**
- Kata yang emang nggak ada padanan enaknya: *vibes, effort, deadline, meeting, random, literally, prefer, mood, insecure, overthinking.*
- Kata sambung khas "anak Jaksel": *which is, basically, literally, honestly, at least, anyway.*
- Ungkapan pendek: *"Same."*, *"Mood."*, *"It's giving..."*, *"No offense, tapi..."*

**Aturan:**
1. **Code-mixing itu ciri karakter**. Tetapin di voice sheet siapa yang campur Inggris berat, siapa yang nggak sama sekali.
2. **Struktur kalimat tetap Indonesia.** "Gue *prefer* yang ini sih" ✅. "I prefer this one, sih" (full Inggris + partikel) cuma buat karakter Jaksel ekstrem.
3. **Maksimal 1–2 kata Inggris per kalimat** di level 2.
4. **Imbuhan Indonesia ke kata Inggris pakai strip**: *di-cancel, nge-spill, di-ghosting, ke-trigger, overthinking-nya.*
5. **Italic**: ikutin `italic_kata_asing` di Style Lock. Default: kata yang udah umum (*vibes, healing, baper*) nggak usah dimiringin; ungkapan panjang atau jarang dipakai dimiringin. **Konsisten** dari bab 1.

---

## 9. Narasi vs Dialog vs Batin vs Chat

Empat "mode" ini punya aturan beda. Jangan ketuker.

| Mode | Level slang | Singkatan | Partikel | Catatan |
|---|---|---|---|---|
| **Narasi** | Sesuai Style Lock | ❌ | Dikit | POV 1 lebih bebas; POV 3 lebih rapi |
| **Dialog** | Style Lock ± 1 sesuai karakter | ❌ | ✅ | Harus kedengeran kayak ngomong |
| **Batin** (italic) | Bisa paling liar | Jarang | ✅ | Tempat tokoh jujur & nyeleneh |
| **Chat** | Level 3 boleh | ✅ | ✅ | Format khusus (lihat bagian 11) |

**POV 1 (gue/aku):** narasi = curhatan tokoh. Boleh nyeletuk, nyindir, ngomong ke pembaca.

> Gue benci hari Senin. Bukan benci biasa, tapi benci yang level *pengen pindah planet*.

**POV 3:** narasi lebih kalem, slang dikurangin satu level, tapi tetep pakai ejaan santai dan kalimat pendek. Celetukan tokoh disalurin lewat batin/dialog.

> Raka mendengus. Lagi-lagi Senin, lagi-lagi telat. *Kenapa sih Senin harus ada.*

---

## 10. Teknik Nulis ala Wattpad

### 10.1 Hook (Kalimat Pembuka)

Kalimat pertama tiap bab harus bikin orang nggak bisa berhenti. Pilih salah satu:

| Jenis | Contoh |
|---|---|
| Pernyataan nyeleneh | "Kalau aja waktu itu gue nggak salah masuk toilet cowok, hidup gue nggak bakal se-chaos ini." |
| In media res (langsung di tengah aksi) | "Gue lari sekenceng-kencengnya sambil nenteng sebelah sepatu cowok yang barusan bikin gue hampir di-DO." |
| Dialog mengejutkan | "'Lo tau nggak, kita tuh sebenernya udah tunangan dari kecil?'" |
| Notif HP | "**1 pesan baru dari: Mantan 🚩**" |
| Pengakuan | "Oke, gue ngaku. Gue yang ngerusak motor Kak Dirga." |

❌ **Jangan buka pakai**: bangun tidur + liat jam, deskripsi cuaca, perkenalan diri ala biodata ("Namaku Rara, umurku 17 tahun, aku suka warna pink...").

### 10.2 Cliffhanger (Penutup Bab)

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

### 10.3 Show, Don't Tell

| Tell ❌ | Show ✅ |
|---|---|
| Rian marah banget. | Rian ngegebrak meja kantin sampai kuah baksonya tumpah. |
| Aku gugup. | Gue udah ngetik "hai" terus ngehapus lagi. Tujuh kali. |
| Dia cantik. | Satu kelas mendadak hening pas dia masuk. Bahkan Pak Darto lupa lanjutin absen. |

### 10.4 Dialog yang Hidup

- **Kurangin dialog tag** ("katanya", "tanyanya", "ujarnya"). Ganti pakai **beat** (aksi kecil).

> ❌ "Kamu mau ke mana?" tanya Rara dengan penasaran. "Mau pergi," jawab Dirga dengan sinis.
>
> ✅ "Lo mau ke mana?" Rara berhenti di depan pintu.
>
> Dirga cuma ngelirik sekilas sambil masang helm. "Ke mana aja yang nggak ada lo."

- Kalau tag diperlukan, pakai yang simpel: **kata, tanya, bisik, teriak**. Jangan "ujarnya dengan nada penuh amarah yang membara".
- Orang nyata **motong omongan**, **nggak selesai ngomong**, **jawab nggak nyambung**. Pakai itu.
- Jangan ada dialog yang isinya cuma ngasih info ke pembaca ("Seperti yang kamu tahu, kita sudah sahabatan sejak SD dan ayahmu adalah CEO...").

### 10.5 Paragraf & Ritme

- 1–4 kalimat per paragraf. Kasih spasi lega.
- Campur kalimat panjang dan pendek. Kalimat super pendek = efek dramatis.

> Dia pergi.
>
> Gitu aja. Tanpa pamit, tanpa chat, tanpa apa-apa.

- Satu kalimat satu paragraf boleh, tapi jangan tiap paragraf (jadi kayak puisi).

### 10.6 Struktur Bab

| Bagian | Isi | Porsi |
|---|---|---|
| Hook | Kalimat/adegan pembuka yang narik | 5% |
| Bangun | Konflik kecil, interaksi, banter | 60% |
| Naik | Ketegangan/emosi meningkat | 25% |
| Cliffhanger | Gantung | 10% |

Panjang ideal: **1.200–2.000 kata**. Konsisten antarbab.

### 10.7 Trope Wattpad yang Lagi Laku (2025–2026)

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

### 10.8 Author's Note (Opsional)

Kalau diminta nulis A/N, gayanya kayak ngobrol sama pembaca:

> **A/N:** Haii, maaf telat update 😭 minggu ini deadline kampus brutal banget. Btw kalian tim Raka atau tim Dirga? Spill di komen yaa. Jangan lupa vote biar aku semangat lanjutin! 💛

A/N **dipisah** dari isi cerita (pakai garis/judul A/N), jangan nyelip di tengah adegan.

---

## 11. Format & Tanda Baca

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

**Tanda seru & tanya:**
- Maksimal `?!` atau `!!` buat adegan heboh. Jangan `!!!!!!!`.
- Huruf kapital semua cuma buat teriak beneran, dan jarang.

**Emoji:** cuma di chat, sosmed, dan A/N. **Nggak boleh** di narasi dan dialog lisan.

**Angka:** satu sampai sembilan ditulis huruf di narasi ("tiga hari"), kecuali jam, tanggal, harga ("jam 2 pagi", "Rp25 ribu").

---

## 12. Voice Tiap Karakter

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

---

## 13. Contoh Kaku vs Santai

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

## 14. Yang Haram Dilakuin (Anti-Pattern)

### 14.1 Bahasa Kaku / Kerasa "AI Banget"

Hindarin frasa klise dan puitis lebay ini:

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

### 14.2 Slang Overdosis

❌
> "Anjir bestie, literally gue salting parah sih, dia tuh vibes-nya green flag banget which is gue jadi delulu, fr fr, slay!"

Ini nggak lucu, ini capek bacanya. **Maksimal 2–3 slang per kalimat dialog**, itu pun buat karakter yang emang gitu.

### 14.3 Inkonsistensi (Dosa Paling Besar)

- ❌ Bab 1 `gue`, bab 3 tiba-tiba `aku` tanpa alasan.
- ❌ Satu paragraf ada `nggak`, `gak`, dan `tidak` sekaligus.
- ❌ Tokoh pendiem tiba-tiba ngomong kayak tukang roasting.
- ❌ Format chat bab 2 beda sama bab 5.
- ❌ Panggilan berubah-ubah ("Kak Dirga" → "Dirga" → "Bang Dirga") tanpa momen.

### 14.4 Lain-lain

- ❌ Singkatan chat di narasi ("Gue udh capek bgt").
- ❌ Emoji di narasi.
- ❌ Infodump (deskripsi 3 paragraf soal wajah tokoh).
- ❌ Biodata di bab 1.
- ❌ Ngejelasin lelucon atau slang di dalam cerita ("Delulu, yang artinya delusional, adalah...").
- ❌ Slang dipakai salah arti (misal "gabut" buat "sibuk").
- ❌ Body shaming, rasis, atau slang peyoratif buat ngehina kelompok — kecuali buat nunjukin karakter itu jahat, dan ceritanya jelas nggak ngebenerin.

---

## 15. Checklist Konsistensi

Jalanin ini tiap selesai nulis satu bab:

- [ ] Kata ganti narasi sama kayak Style Lock?
- [ ] Kata ganti tiap karakter sama kayak voice sheet?
- [ ] Ejaan negasi cuma satu versi (`nggak` / `gak` / `enggak`)?
- [ ] Nggak ada campuran `udah/sudah`, `aja/saja`, `kayak/seperti` di dialog?
- [ ] Level slang narasi sesuai Style Lock?
- [ ] Singkatan cuma muncul di adegan chat?
- [ ] Emoji cuma di chat/A/N?
- [ ] Italic kata asing konsisten?
- [ ] Format chat & pemisah adegan sama kayak bab sebelumnya?
- [ ] Panggilan antar karakter konsisten?
- [ ] Bab dibuka pakai hook?
- [ ] Bab ditutup pakai cliffhanger / pertanyaan ngegantung?
- [ ] Paragraf maksimal 4 kalimat?
- [ ] Ada minimal satu momen show-don't-tell yang kuat?
- [ ] Nggak ada frasa "AI banget" dari bagian 14.1?
- [ ] Adegan serius udah turunin slang?
- [ ] Kata kasar sesuai rating?
- [ ] Panjang bab di kisaran target?

---

## 16. Cara Agent Pakai Skill Ini

Skill ini dibikin biar bisa dipakai **banyak agent** sekaligus (penulis, editor, reviewer, dll). Biar hasilnya seragam, semua agent ikutin alur ini:

### 16.1 Alur Kerja

1. **Cek konteks.** Ini cerita baru atau lanjutan?
   - **Baru** → bikin Style Lock + voice sheet dulu (pakai default kalau user nggak nentuin).
   - **Lanjutan** → baca bab sebelumnya, **simpulin Style Lock dari tulisan yang udah ada**, jangan bikin gaya baru.
2. **Tulis** sesuai Style Lock dan aturan di skill ini.
3. **Self-check** pakai checklist di bagian 15.
4. **Output** sesuai format di bawah.

### 16.2 Peran Agent

| Peran | Tugas |
|---|---|
| **Penulis** | Nulis bab/adegan baru sesuai Style Lock. |
| **Editor gaya** | Ngubah tulisan kaku jadi santai tanpa ngubah plot. Fokus ke bagian 4, 5, 13, 14. |
| **Reviewer konsistensi** | Nyari pelanggaran pakai checklist bagian 15, kasih daftar temuan + saran perbaikan per baris. |
| **Penulis chat scene** | Fokus ke bagian 7 & format chat bagian 11. |

### 16.3 Format Output

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
| "Aku tidak tau..." | Kata ganti & negasi nggak sesuai Style Lock | "Gue nggak tau..." |
```

### 16.4 Aturan Prioritas

Kalau ada yang bentrok, ikutin urutan ini:
1. Instruksi langsung dari user.
2. Gaya bab-bab yang udah ditulis sebelumnya (konsistensi cerita).
3. Style Lock & voice sheet.
4. Default di skill ini.

### 16.5 Update Slang

Slang 🔴 tren cepet basi. Kalau agent punya akses internet dan user minta "biar makin kekinian", boleh nyari slang terbaru, tapi:
- Pastiin artinya bener (cek minimal 2 sumber).
- Kasih label 🟢/🟡/🔴/⚫ sebelum dipakai.
- Jangan ubah slang di bab yang udah jadi, kecuali diminta.

---

<div align="center">

*Skill ini fokus ke gaya bahasa cerita. Tetep di jalur, jangan OOT. Gas nulis! ✍️*

<sub>Dirilis dengan lisensi <a href="LICENSE">MIT</a> — bebas dipakai, diubah, dan dikomersialkan.</sub>

</div>
