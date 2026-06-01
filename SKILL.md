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
- Setiap kali ada perubahan kode, feature

## How I Do It

1. Baca file progress.txt untuk melihat log terakhir
2. Append entry baru di bagian bawah file
3. Group berdasarkan tanggal, gunakan bullet points
4. Format : aksi ('Modified','Created','Deleted','Fixed') + Nama File + Deskripsi Singkat

## Log Format

### YYYY-MM-DD

- **Modified**: NamaFile.\*extension - Deskripsi Singkat
- **Created**: NamaFile.\*extension - Deskripsi Singkat
- **Deleted**: NamaFile.\*extension - Deskripsi Singkat
- **Fixed**: NamaFile.\*extension - Deskripsi Singkat

**PENTING**

- Selalu append,jangan overwrite file yang sudah ada
