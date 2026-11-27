# Changelog

Semua perubahan penting di skill ini dicatet di sini.
Format mengikuti [Keep a Changelog](https://keepachangelog.com/id-ID/1.1.0/) dan versi mengikuti [Semantic Versioning](https://semver.org/lang/id/).

## [Unreleased]

### Added
- Dukungan **Hosted Remote MCP Server** publik di `https://humanizer-id.mbsc.my.id/mcp` (Streamable HTTP stateless, auto-sync file `.md` dari GitHub, 5 tools + Resources + Prompts).
- Tampilan `README.md` baru yang lebih rapi: hero CTA, 3 contoh before/after, tabel level slang, panduan koneksi MCP (ChatGPT, Claude Code, Antigravity, Cursor), dan bagian Sponsor & Support.

## [2.0.0] - 2026-11-26

### Changed
- **BREAKING:** skill di-rename dari `gayabahasa` jadi `humanizer-id`, dan cakupannya diperluas dari khusus nulis cerita jadi multifungsi.
- `SKILL.md` sekarang jadi inti aturan + pemilih mode di root repo. Materi spesifik tiap kebutuhan dipindah ke `modes/`.
- Style Lock diganti jadi **Tone Lock** (berlaku buat semua mode, bukan cuma cerita).
- Kamus slang dan singkatan dipindah ke `references/kamus-slang.md`.
- Materi nulis cerita (hook, cliffhanger, voice sheet, format, contoh) dipindah ke `modes/cerita.md`.
- Aturan singkatan chat sekarang per mode, bukan cuma buat adegan chat di cerita.

### Added
- Level slang 0 (**Santai Sopan**) buat CS, klien, atasan, dan topik sensitif.
- 7 mode baru: `humanizer`, `sosmed`, `copywriting`, `chatbot`, `chat-harian`, `artikel`, `terjemahan`.
- Bagian **Peka Konteks** (duka, sakit, duit/komplain, SARA, atasan/klien).
- Anti-pattern "kerasa AI" buat tulisan non-fiksi.
- Tabel pilih kata ganti (`gue-lo`, `aku-kamu`, `kamu`, `Kak`, `Anda`).
- Aturan prioritas multi-agent yang diperluas.
- Packaging multi-platform di root repo (siap langsung download `main.zip` dan upload):
  - `.claude-plugin/plugin.json` & `.claude-plugin/marketplace.json` (Claude Code & ChatGPT)
  - `.cursor-plugin/plugin.json` (Cursor)
  - `agents/openai.yaml` (OpenAI / Codex)
  - `package.json` (Pi)
- README baru: tabel mode, contoh prompt per mode, dan link download ZIP langsung dari GitHub.

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
