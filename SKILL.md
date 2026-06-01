---
name: log-skill
description: Log Pekerjaan yang sudah dikerjakan
license: MIT
compatibility: opencode
metadata:
  audience: maintainers
---

## What I do

- Tambahkan log yang sudah dikerjakan di file progress.txt

## When to use me

- Setelah selesai membuat file, refactor, menjalankan task dan memperbaiki bug
- Setiap kali ada perubahan kode, feature, konfigurasi env, atau dependency

## How I Do It

1. Baca file progress.txt untuk melihat log terakhir
2. Append entry baru di bagian bawah file
3. Group berdasarkan tanggal, gunakan bullet points
4. Format: aksi ('Modified','Created','Deleted','Fixed') + [Scope] Nama File - Deskripsi Singkat

## Log Format & Scopes

### Scopes:
- `[FE/Page]`: Halaman di `src/app`
- `[FE/Component]`: Komponen UI di `src/components`
- `[FE/Hook]`: Hooks custom di `src/hooks`
- `[FE/Lib]`: Helper/API Client di `src/lib`
- `[BE/Controller]`: API backend di PHP/CI3
- `[Config]`: File konfigurasi (`package.json`, `.env.local`, `next.config.ts`, dll.)

### Format Entry:
- **Created**: `[Scope]` NamaFile.*ext - Deskripsi
- **Modified**: `[Scope]` NamaFile.*ext - Deskripsi
- **Fixed**: `[Scope]` NamaFile.*ext - Deskripsi
- **Deleted**: `[Scope]` NamaFile.*ext - Deskripsi

*Note: Jika ada instalasi library baru atau perubahan skema API, cantumkan detailnya di bawah baris terkait.*

### YYYY-MM-DD

- **Modified**: `[Scope]` NamaFile.*ext - Deskripsi Singkat
- **Created**: `[Scope]` NamaFile.*ext - Deskripsi Singkat
- **Deleted**: `[Scope]` NamaFile.*ext - Deskripsi Singkat
- **Fixed**: `[Scope]` NamaFile.*ext - Deskripsi Singkat

**PENTING**

- Selalu append, jangan overwrite file yang sudah ada
