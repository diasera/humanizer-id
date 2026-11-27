<div align="center">

# ✍️ humanizer-id

**Humanizer versi Indonesia 🇮🇩 — skill AI agent multifungsi buat bikin tulisan bahasa Indonesia santai, natural, dan kekinian ala Gen Z 2026. Cocok buat cerita, sosmed, copywriting, chatbot, chat harian, artikel, sampai terjemahan. Santai, nggak kaku, dan konsisten.**

[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![Bahasa](https://img.shields.io/badge/bahasa-Indonesia-red.svg)
![Format](https://img.shields.io/badge/format-SKILL.md-8A2BE2.svg)
![Plugin](https://img.shields.io/badge/plugin-ChatGPT%20%7C%20Codex%20%7C%20Claude%20%7C%20Antigravity-orange.svg)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[Fitur](#-fitur) •
[Mode](#-mode-yang-tersedia) •
[Preview](#-preview) •
[Cara Pakai](#-cara-pakai) •
[Contoh Prompt](#-contoh-prompt) •
[Kontribusi](#-kontribusi) •
[Lisensi](#-lisensi)

</div>

---

## 🤔 Ini Apa?

`humanizer-id` adalah **skill (instruksi siap pakai)** buat AI agent — Antigravity, Claude Code, Cursor, ChatGPT, Gemini, dan agent lain yang bisa baca file Markdown.

Pernah nyuruh AI nulis sesuatu terus hasilnya kayak gini?

> *"Dalam era digital yang terus berkembang pesat ini, penting bagi kita untuk memahami bahwa manajemen waktu merupakan kunci utama kesuksesan."*

Kaku. Lebay. Kerasa banget AI-nya. 😮‍💨

Skill ini ngajarin agent buat nulis kayak **anak umur 20-25 tahun yang lagi ngobrol**: pakai bahasa sehari-hari, slang Gen Z yang pas, dan yang paling penting, **gayanya nggak berubah-ubah** dari awal sampai akhir.

Bedanya sama skill "humanizer" biasa: `humanizer-id` **multifungsi**. Satu inti aturan, **8 mode** buat kebutuhan yang beda-beda. Bisa buat nulis novel, caption IG, deskripsi produk, persona CS, sampai balas chat.

---

## ✨ Fitur

| | Fitur | Penjelasan |
|---|---|---|
| 🔌 | **Plugin Siap Pasang** | Bisa dipasang sebagai plugin di ChatGPT/Codex, Claude Code, dan Antigravity, atau sebagai skill biasa. |
| 🧩 | **8 Mode** | Cerita, humanizer, sosmed, copywriting, chatbot, chat harian, artikel, terjemahan. Tiap mode punya default, contoh, dan checklist sendiri. |
| 🔒 | **Tone Lock** | Kartu gaya (kata ganti, level slang, ejaan, emoji) yang dikunci dari awal biar konsisten. |
| 🎚️ | **4 Level Slang (0–3)** | Dari santai sopan sampai full Gen Z, otomatis turun di topik serius. |
| 📖 | **Kamus Slang 2026** | 100+ istilah dengan arti, contoh, dan label umur kata (🟢 evergreen, 🟡 umum, 🔴 tren, ⚫ kasar). |
| 💬 | **Singkatan dan Gaya Chat** | `yg`, `bgt`, `ngl`, `fr`, `ygy`, sampai arti emoji 😭💀, plus aturan kapan boleh dipakai per mode. |
| 🫶 | **Peka Konteks** | Duka, komplain, urusan duit, atau ngomong ke atasan? Slang otomatis diturunin. |
| 🚫 | **Anti-Pattern** | Daftar frasa klise "AI banget" dan cara gantinya. |
| ✅ | **Checklist** | Checklist umum + checklist per mode buat ngecek hasil. |
| 🤖 | **Multi-Agent Ready** | Peran penulis, editor, reviewer, dan format output yang seragam. |

---

## 🧩 Mode yang Tersedia

| Mode | Buat apa | File | Contoh pemakaian |
|---|---|---|---|
| 📚 **Cerita** | Novel, Wattpad, cerbung, fanfic, AU | [cerita.md](plugins/humanizer-id/skills/humanizer-id/modes/cerita.md) | "Tulis bab 1 romcom kampus, POV gue." |
| 🧑‍💻 **Humanizer** | Ubah teks kaku/kerasa AI jadi natural | [humanizer.md](plugins/humanizer-id/skills/humanizer-id/modes/humanizer.md) | "Ubah paragraf ini biar nggak kaku." |
| 📱 **Sosmed** | Caption IG/TikTok, thread, script video | [sosmed.md](plugins/humanizer-id/skills/humanizer-id/modes/sosmed.md) | "Bikin caption buat kafe baru." |
| 🛍️ **Copywriting** | Iklan, promo, deskripsi produk, push notif | [copywriting.md](plugins/humanizer-id/skills/humanizer-id/modes/copywriting.md) | "Deskripsi tas ransel buat marketplace." |
| 🤖 **Chatbot** | Persona chatbot dan customer service | [chatbot.md](plugins/humanizer-id/skills/humanizer-id/modes/chatbot.md) | "Bikin persona CS yang ramah buat toko online." |
| 💬 **Chat harian** | Balas WA, DM, komen | [chat-harian.md](plugins/humanizer-id/skills/humanizer-id/modes/chat-harian.md) | "Bantuin nolak ajakan nongki dengan halus." |
| 📰 **Artikel** | Blog, artikel, newsletter | [artikel.md](plugins/humanizer-id/skills/humanizer-id/modes/artikel.md) | "Artikel tips hemat anak kos." |
| 🌐 **Terjemahan** | Teks baku/Inggris → bahasa gaul | [terjemahan.md](plugins/humanizer-id/skills/humanizer-id/modes/terjemahan.md) | "Terjemahin pengumuman ini jadi gaul." |

Aturan inti, ejaan, level slang, dan checklist umum ada di [SKILL.md](plugins/humanizer-id/skills/humanizer-id/SKILL.md). Daftar kata dan singkatan ada di [references/kamus-slang.md](plugins/humanizer-id/skills/humanizer-id/references/kamus-slang.md).

---

## 👀 Preview

### Mode Cerita

<table>
<tr>
<th width="50%">❌ Sebelum (kaku)</th>
<th width="50%">✅ Sesudah (pakai skill ini)</th>
</tr>
<tr>
<td valign="top">

Pagi itu, aku terbangun dengan perasaan yang tidak menentu. Matahari bersinar dengan cerahnya, namun hatiku diselimuti oleh mendung yang kelabu. Aku sangat merindukan dirinya yang telah pergi meninggalkanku.

</td>
<td valign="top">

Gue bangun jam sepuluh, dan hal pertama yang gue lakuin adalah ngecek HP.

Nggak ada chat dari dia. Lagi.

Gue lempar HP ke kasur, terus narik selimut sampai nutup muka. Di luar cerah banget, kayak semesta lagi ngeledek. *Iya, iya, cuma gue doang yang gamon di sini.*

</td>
</tr>
</table>

### Mode Humanizer

<table>
<tr>
<th width="50%">❌ Sebelum (kerasa AI)</th>
<th width="50%">✅ Sesudah (level 1)</th>
</tr>
<tr>
<td valign="top">

Dalam era digital yang terus berkembang pesat ini, penting bagi kita untuk memahami bahwa manajemen waktu merupakan kunci utama dalam mencapai produktivitas yang optimal. Dengan menerapkan strategi yang tepat, kita dapat menyelesaikan berbagai tugas secara efisien dan efektif.

</td>
<td valign="top">

Kalau waktu kamu berantakan, kerjaan ikut berantakan. Makanya ngatur waktu itu penting banget. Tentuin dulu mana yang paling mendesak, kerjain satu-satu, dan sisain waktu buat istirahat.

</td>
</tr>
</table>

---

## 🚀 Cara Pakai

> [!TIP]
> Cara paling gampang: pasang sebagai **plugin**. Skill, semua mode, dan kamus langsung ikut dalam satu paket.

### Plugin: ChatGPT / Codex

Repo ini udah punya marketplace (`.agents/plugins/marketplace.json`). Tambahin repo `diasera/humanizer-id` sebagai marketplace lewat menu **Plugins**, terus install `humanizer-id`.

Kalau repo ini di-clone dan dibuka di Codex, marketplace-nya otomatis kebaca.

> [!NOTE]
> Nama menu bisa beda tergantung versi aplikasinya.

### Plugin: Claude Code

```
/plugin marketplace add diasera/humanizer-id
/plugin install humanizer-id@humanizer-id
```

### Plugin: Google Antigravity

Copy folder `plugins/humanizer-id/` ke folder plugin Antigravity:

```
~/.gemini/config/plugins/humanizer-id/
```

Di Windows: `%USERPROFILE%\.gemini\config\plugins\humanizer-id\`

### Skill biasa (tanpa plugin)

Copy folder `plugins/humanizer-id/skills/humanizer-id/` ke:

```
# Antigravity
.agents/skills/humanizer-id/

# Claude Code (per project / global)
.claude/skills/humanizer-id/
~/.claude/skills/humanizer-id/
```

Atau pakai `skills` CLI:

```bash
npx skills add diasera/humanizer-id
```

> [!IMPORTANT]
> Pasang **seluruh folder skill** (`SKILL.md` + `modes/` + `references/`), bukan cuma `SKILL.md`. File mode dan kamus dipanggil dari `SKILL.md`.

### Upload manual (Custom GPT / Gemini Gems / Claude Projects)

Upload **semua file `.md`** di `plugins/humanizer-id/skills/humanizer-id/` sebagai **knowledge file**. Atau copy-paste isi `SKILL.md` ke **instructions** dan upload sisanya sebagai knowledge.

### Manual

```bash
git clone https://github.com/diasera/humanizer-id.git
```

Terus pakai folder-nya di mana aja kamu butuh.

---
## 💡 Contoh Prompt

```text
[Cerita] Pakai skill humanizer-id. Tulis bab 1 cerita romcom kampus, POV gue,
enemies to lovers, level slang 2, sekitar 1.500 kata.
```

```text
[Humanizer] Pakai skill humanizer-id. Ubah teks ini biar nggak kaku dan nggak
kerasa AI, jangan ubah isinya: [tempel teks]
```

```text
[Sosmed] Pakai skill humanizer-id. Bikin caption IG buat kafe baru buka di
Bandung, tone santai, ada CTA, 4 hashtag.
```

```text
[Copywriting] Pakai skill humanizer-id. Tulis deskripsi produk tas ransel anti
air 20 liter buat marketplace, tone santai tapi tetap jujur.
```

```text
[Chatbot] Pakai skill humanizer-id. Bikin persona chatbot CS toko skincare:
ramah, panggil user "Kak", dan tau kapan harus serius.
```

```text
[Chat harian] Pakai skill humanizer-id. Bantuin bales chat temen yang ngajak
nongki malam ini, padahal gue capek. Kasih 3 opsi.
```

```text
[Artikel] Pakai skill humanizer-id. Tulis artikel blog 600 kata soal tips hemat
anak kos, gaya santai tapi informatif.
```

```text
[Terjemahan] Pakai skill humanizer-id. Terjemahin teks ini ke bahasa Indonesia
gaul (level 2), nama dan angka jangan berubah: [tempel teks]
```

---

## 📂 Struktur Repo

```
humanizer-id/
├── .agents/plugins/marketplace.json   # marketplace ChatGPT / Codex
├── .claude-plugin/marketplace.json    # marketplace Claude Code
├── plugins/
│   └── humanizer-id/                  # plugin-nya
│       ├── plugin.json                # manifest Antigravity
│       ├── .codex-plugin/plugin.json  # manifest ChatGPT / Codex
│       ├── .claude-plugin/plugin.json # manifest Claude Code
│       ├── LICENSE
│       └── skills/
│           └── humanizer-id/
│               ├── SKILL.md           # inti skill + pilih mode (dibaca agent)
│               ├── modes/
│               │   ├── cerita.md      # novel, Wattpad, fanfic
│               │   ├── humanizer.md   # ubah teks kaku/AI jadi natural
│               │   ├── sosmed.md      # caption, thread, script video
│               │   ├── copywriting.md # iklan, promo, deskripsi produk
│               │   ├── chatbot.md     # persona chatbot / CS
│               │   ├── chat-harian.md # balas WA, DM, komen
│               │   ├── artikel.md     # blog, artikel, newsletter
│               │   └── terjemahan.md  # baku/Inggris → gaul
│               └── references/
│                   └── kamus-slang.md # kamus slang dan singkatan
├── README.md                          # yang lagi kamu baca
├── CONTRIBUTING.md                    # cara nambah slang / mode
├── CHANGELOG.md                       # riwayat versi
└── LICENSE                            # MIT
```

---
## 📚 Isi Skill

<details>
<summary><b>Klik buat liat daftar isi lengkap <code>SKILL.md</code></b></summary>

1. Cara Kerja
2. Pilih Mode
3. Aturan Emas
4. Tone Lock
5. Level Slang
6. Ejaan Santai yang Udah Dikunci
7. Partikel Bahasa Lisan
8. Campur Bahasa Inggris
9. Kamus Slang dan Singkatan
10. Peka Konteks
11. Anti-Pattern Umum
12. Checklist Umum
13. Kerja Bareng Banyak Agent

</details>

---

## 🤝 Kontribusi

Slang itu cepet banget berubah. Kalau nemu istilah baru, arti yang kurang pas, slang yang udah basi, atau mau nambah mode baru, **PR dan issue sangat diterima!**

Baca dulu [CONTRIBUTING.md](CONTRIBUTING.md) biar formatnya seragam.

---

## ⚠️ Disclaimer

- Slang berlabel 🔴 **tren** gampang basi. Cek ulang sebelum dipakai buat konten jangka panjang.
- Beberapa istilah berlabel ⚫ bersifat **kasar/peyoratif**. Istilah itu dicantumin cuma buat kebutuhan karakter fiksi, bukan buat ngehina siapa pun.
- Arti slang dikumpulin dari pemakaian sehari-hari dan sumber publik (artikel gaya hidup, media sosial). Pemakaian bisa beda-beda tiap daerah dan circle.
- **Etika humanizer:** skill ini buat bikin tulisan enak dibaca, **bukan** buat nyontek tugas akademik atau ngaku tulisan orang lain sebagai karya sendiri. Skill ini juga **nggak menjamin** tulisan lolos AI detector.
- Skill ini buat teks santai. Jangan dipakai buat dokumen hukum, medis, atau akademik formal.

---

## 📄 Lisensi

Dirilis dengan lisensi **[MIT](LICENSE)** © 2026 diasera.

Artinya kamu **bebas** pakai, ubah, gabungin, publikasi, distribusi, sublisensi, bahkan **jual** — buat proyek pribadi maupun **komersial**. Syaratnya cuma satu: **cantumin file `LICENSE` / copyright notice** di salinan kamu.

<div align="center">

---

Kalau skill ini kepake, kasih ⭐ ya biar makin banyak yang nemu!

**Gas nulis! ✍️**

</div>
