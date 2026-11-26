<div align="center">

# ✍️ humanizer-id

**Humanizer versi Indonesia 🇮🇩 — skill AI agent buat nulis cerita Wattpad & novel pakai bahasa Indonesia Gen Z 2026 — santai, nggak kaku, dan konsisten dari bab 1 sampai tamat.**

[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Bahasa](https://img.shields.io/badge/bahasa-Indonesia-red.svg)
![Format](https://img.shields.io/badge/format-SKILL.md-8A2BE2.svg)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[Fitur](#-fitur) •
[Preview](#-preview) •
[Cara Pakai](#-cara-pakai) •
[Contoh Prompt](#-contoh-prompt) •
[Kontribusi](#-kontribusi) •
[Lisensi](#-lisensi)

</div>

---

## 🤔 Ini Apa?

`humanizer-id` adalah **skill (instruksi siap pakai)** buat AI agent — Antigravity, Claude Code, Cursor, ChatGPT, Gemini, dan agent lain yang bisa baca file Markdown.

Pernah nyuruh AI nulis cerita terus hasilnya kayak gini?

> *"Di tengah hiruk-pikuk kota, jantungku berdegup kencang tak karuan, seolah-olah dunia berhenti berputar."*

Kaku. Lebay. Kerasa banget AI-nya. 😮‍💨

Skill ini ngajarin agent buat nulis kayak **anak umur 20-25 tahun yang lagi cerita** — pakai bahasa sehari-hari, slang Gen Z yang pas, dan yang paling penting: **gayanya nggak berubah-ubah** antarbab.

---

## ✨ Fitur

| | Fitur | Penjelasan |
|---|---|---|
| 🔒 | **Style Lock** | Kartu gaya (POV, `gue-lo`/`aku-kamu`, level slang, ejaan) yang dikunci dari awal biar konsisten. |
| 🎚️ | **3 Level Slang** | Dari santai ringan sampai full Gen Z, otomatis turun di adegan serius. |
| 📖 | **Kamus Slang 2026** | 100+ istilah dengan arti, contoh, dan label umur kata (🟢 evergreen, 🟡 umum, 🔴 tren, ⚫ kasar). |
| 💬 | **Singkatan & Format Chat** | `yg`, `bgt`, `ngl`, `fr`, `ygy`, sampai arti emoji 😭💀 — plus aturan kapan boleh dipakai. |
| 🗣️ | **Voice Sheet Karakter** | Template biar tiap tokoh punya cara ngomong sendiri. |
| 🪝 | **Teknik Wattpad** | Hook, cliffhanger, show don't tell, dialog beat, struktur bab, trope yang lagi laku. |
| 🚫 | **Anti-Pattern** | Daftar frasa klise "AI banget" dan cara gantinya. |
| ✅ | **Checklist Konsistensi** | 18 poin yang dicek tiap selesai satu bab. |
| 🤖 | **Multi-Agent Ready** | Peran penulis, editor, reviewer, dan format output yang seragam. |

---

## 👀 Preview

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

---

## 🚀 Cara Pakai

### Pakai `skills` CLI (paling gampang)

```bash
npx skills add diasera/humanizer-id
```

### Google Antigravity

Taruh file di folder skill workspace kamu:

```
.agents/skills/humanizer-id/SKILL.md
```

### Claude Code

```
# per project
.claude/skills/humanizer-id/SKILL.md

# global (semua project)
~/.claude/skills/humanizer-id/SKILL.md
```

### Cursor / Windsurf / agent lain

Simpen isi `SKILL.md` sebagai rule/instruksi project (misal di folder `.cursor/rules/`), atau tinggal sebut file-nya di prompt.

### ChatGPT (Custom GPT) / Gemini (Gems) / Claude Projects

Upload `SKILL.md` sebagai **knowledge file**, atau copy-paste isinya ke **instructions**.

### Manual

```bash
git clone https://github.com/diasera/humanizer-id.git
```

Terus pakai `SKILL.md` di mana aja kamu butuh.

---

## 💡 Contoh Prompt

```text
Pakai skill humanizer-id. Tulis bab 1 cerita romcom kampus, POV gue,
enemies to lovers, level slang 2, sekitar 1.500 kata.
```

```text
Pakai skill humanizer-id sebagai editor gaya. Ubah bab ini biar nggak kaku,
jangan ubah plotnya: [tempel teks]
```

```text
Pakai skill humanizer-id sebagai reviewer konsistensi. Cek bab 5 ini
dibandingin sama bab 1-4, kasih tabel temuan dan saran perbaikan.
```

```text
Pakai skill humanizer-id. Bikinin adegan chat WA antara Raka (tengil,
level slang 3) dan Nadia (kalem, aku-kamu) pas Raka ketahuan bohong.
```

---

## 📂 Struktur Repo

```
humanizer-id/
├── SKILL.md          # skill utama (ini yang dibaca agent)
├── README.md         # yang lagi kamu baca
├── CONTRIBUTING.md   # cara nambah slang / ngasih masukan
├── CHANGELOG.md      # riwayat versi
└── LICENSE           # MIT
```

---

## 📚 Isi Skill

<details>
<summary><b>Klik buat liat daftar isi lengkap <code>SKILL.md</code></b></summary>

1. Aturan Emas (Wajib Banget)
2. Kunci Gaya Dulu Sebelum Nulis (Style Lock)
3. Level Slang
4. Ejaan Santai yang Udah Dikunci
5. Partikel: Nyawanya Bahasa Lisan
6. Kamus Slang Gen Z 2026
7. Singkatan Chat
8. Campur Bahasa Inggris (Code-Mixing)
9. Narasi vs Dialog vs Batin vs Chat
10. Teknik Nulis ala Wattpad
11. Format & Tanda Baca
12. Voice Tiap Karakter
13. Contoh Kaku vs Santai
14. Yang Haram Dilakuin (Anti-Pattern)
15. Checklist Konsistensi
16. Cara Agent Pakai Skill Ini

</details>

---

## 🤝 Kontribusi

Slang itu cepet banget berubah. Kalau nemu istilah baru, arti yang kurang pas, atau slang yang udah basi, **PR dan issue sangat diterima!**

Baca dulu [CONTRIBUTING.md](CONTRIBUTING.md) biar formatnya seragam.

---

## ⚠️ Disclaimer

- Slang berlabel 🔴 **tren** gampang basi. Cek ulang sebelum dipakai buat cerita jangka panjang.
- Beberapa istilah berlabel ⚫ bersifat **kasar/peyoratif**. Istilah itu dicantumin cuma buat kebutuhan karakter fiksi, bukan buat ngehina siapa pun.
- Arti slang dikumpulin dari pemakaian sehari-hari dan sumber publik (artikel gaya hidup, media sosial). Pemakaian bisa beda-beda tiap daerah dan circle.

---

## 📄 Lisensi

Dirilis dengan lisensi **[MIT](LICENSE)** © 2026 diasera.

Artinya kamu **bebas** pakai, ubah, gabungin, publikasi, distribusi, sublisensi, bahkan **jual** — buat proyek pribadi maupun **komersial**. Syaratnya cuma satu: **cantumin file `LICENSE` / copyright notice** di salinan kamu.

<div align="center">

---

Kalau skill ini kepake, kasih ⭐ ya biar makin banyak yang nemu!

**Gas nulis! ✍️**

</div>
