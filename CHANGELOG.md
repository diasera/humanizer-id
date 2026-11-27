# Changelog

Semua perubahan penting di skill ini dicatet di sini.
Format mengikuti [Keep a Changelog](https://keepachangelog.com/id-ID/1.1.0/) dan versi mengikuti [Semantic Versioning](https://semver.org/lang/id/).

## [Unreleased]

## [2.0.0] - 2026-11-26

### Changed
- **BREAKING:** skill di-rename dari `gayabahasa` jadi `humanizer-id`, dan cakupannya diperluas dari khusus nulis cerita jadi multifungsi.
- `SKILL.md` sekarang jadi inti aturan + pemilih mode. Materi spesifik tiap kebutuhan dipindah ke `modes/`.
- Style Lock diganti jadi **Tone Lock** (berlaku buat semua mode, bukan cuma cerita).
- Kamus slang dan singkatan dipindah ke `references/kamus-slang.md`.
- Materi nulis cerita (hook, cliffhanger, voice sheet, format, contoh) dipindah ke `modes/cerita.md`.
- Aturan singkatan chat sekarang per mode, bukan cuma buat adegan chat di cerita.
- File skill dipindah ke `plugins/humanizer-id/skills/humanizer-id/` (`SKILL.md`, `modes/`, `references/`).

### Added
- Level slang 0 (**Santai Sopan**) buat CS, klien, atasan, dan topik sensitif.
- 7 mode baru: `humanizer`, `sosmed`, `copywriting`, `chatbot`, `chat-harian`, `artikel`, `terjemahan`.
- Bagian **Peka Konteks** (duka, sakit, duit/komplain, SARA, atasan/klien).
- Anti-pattern "kerasa AI" buat tulisan non-fiksi.
- Tabel pilih kata ganti (`gue-lo`, `aku-kamu`, `kamu`, `Kak`, `Anda`).
- Aturan prioritas multi-agent yang diperluas.
- Packaging plugin buat ChatGPT/Codex (`.codex-plugin/plugin.json`), Claude Code (`.claude-plugin/plugin.json`), dan Antigravity (`plugin.json`).
- Marketplace di repo: `.agents/plugins/marketplace.json` (ChatGPT/Codex) dan `.claude-plugin/marketplace.json` (Claude Code).
- README baru: tabel mode, contoh prompt per mode, dan panduan pasang seluruh folder.

## [1.0.0] - 2026-11-26

### Added
- Rilis pertama `SKILL.md`.
- Style Lock & default gaya.
- 3 level slang.
- Tabel ejaan santai yang dikunci.
- Panduan partikel lisan.
- Kamus slang Gen Z 2026 dengan label umur kata (🟢 🟡 🔴 ⚫).
- Daftar singkatan & gaya ketik chat.
- Aturan code-mixing Indonesia–Inggris.
- Aturan mode narasi, dialog, batin, dan chat.
- Teknik nulis Wattpad (hook, cliffhanger, show don't tell, dialog beat, struktur bab, trope).
- Format & tanda baca.
- Template voice sheet karakter.
- Contoh tulisan kaku vs santai.
- Daftar anti-pattern.
- Checklist konsistensi.
- Panduan pemakaian multi-agent.
