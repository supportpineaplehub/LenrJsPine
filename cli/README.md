# 🍍 PineQuiz CLI - Latihan Soal Langsung dari Terminal

[![PineQuiz Version](https://img.shields.io/badge/version-1.0.0-blue)](https://pypi.org/project/pinequiz/)
[![Made with Python](https://img.shields.io/badge/Made%20with-Python-blue?logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Terminal-lightgrey?logo=windows-terminal)](#)

---

## 📘 Introduction

**PineQuiz CLI** adalah sistem kuis interaktif langsung dari terminal!  
Tujuannya? Supaya kamu belajar dengan jujur, tanpa copy-paste jawaban, dan bisa mengasah logika serta pemahaman.

Setiap bab akan memiliki folder `quiz`. Kalau folder itu ada, artinya ada soal yang perlu kamu kerjakan. Kalau tidak, ya tinggalin aja. 😄

📎 Contoh soal `.ps` bisa kamu lihat di sini:  
🔗 [soal.ps (GitHub)](https://github.com/supportpineaplehub/LenrJsPine/blob/main/src/exploreTopics/jsTutorial/jsIntroduction/quiz/soal.ps)

---

## 🛠️ Instalasi

Pastikan Python sudah terinstal. Kalau belum, download di:  
👉 [python.org/downloads](https://www.python.org/downloads/)

Lalu install PineQuiz CLI via pip:

```bash
$ pip install pinequiz
```

---

## 🚀 Cara Penggunaan

### 📦 Format Dasar Perintah:

```bash
$ pinequiz <-cmd> <-flags>
```

🧪 Contoh lihat bantuan:

```bash
$ pinequiz -h
```

📋 Output:

```
🍍 PineQuiz CLI - Latihan Soal Encrypted

options:
  -i, --inti            Mode inti, memulai quiz dari file soal
  -l, --link LINK       Link file .ps dari GitHub (raw URL)
  -x, --execute         Jalankan quiz setelah file diunduh
  -r, --run             Alias dari --execute
  -cfg, --config CONFIG Simpan token GitHub untuk akses privat
  -v, --version         Tampilkan versi CLI
  -h, --helpme          Tampilkan bantuan lengkap
```

---

## 🧠 Mengerjakan Soal Kuis

### 1️⃣ Simpan Token GitHub

```bash
$ pinequiz -cfg GITHUB_TOKEN
```

Contoh:

```bash
$ pinequiz -cfg hdiehpdhihweifhw
```

📥 Respon:

```
✅ Config berhasil disimpan.
```

---

### 2️⃣ Salin Link Soal `.ps`

Contoh link soal:

```
https://raw.githubusercontent.com/supportpineaplehub/LenrJsPine/refs/heads/main/src/exploreTopics/jsTutorial/jsIntroduction/quiz/soal.ps
```

---

### 3️⃣ Jalankan Kuis

```bash
$ pinequiz -i -l "<LINK_SOAL>" -x
```

Contoh lengkap:

```bash
$ pinequiz -i -l "https://raw.githubusercontent.com/supportpineaplehub/LenrJsPine/refs/heads/main/src/exploreTopics/jsTutorial/jsIntroduction/quiz/soal.ps" -x
```

---

## ✅ Output Jika Jawaban Benar

```
📥 Mengunduh soal...
✅ Soal disimpan di: soal_cache\soal.ps

🧠 Soal #1: Jika seorang developer ingin membuat website ...
   a) HTML gak bisa bikin tampilan, harus pakai JavaScript juga
   b) CSS harus ditaruh setelah script JavaScript
   c) Karena belum ada JavaScript buat respon tombolnya
   d) Karena tombolnya harus dibungkus <form> biar jalan
   e) Karena DevTools-nya belum dibuka, jadi gak bisa ngejalanin perintah
Jawaban Anda [a-e]: c
✅ Benar!
```

---

## ❌ Output Jika Jawaban Salah

```
📥 Mengunduh soal...
✅ Soal disimpan di: soal_cache\soal.ps

🧠 Soal #1: Jika seorang developer ingin membuat website ...
   a) HTML gak bisa bikin tampilan, harus pakai JavaScript juga
   b) CSS harus ditaruh setelah script JavaScript
   c) Karena belum ada JavaScript buat respon tombolnya
   d) Karena tombolnya harus dibungkus <form> biar jalan
   e) Karena DevTools-nya belum dibuka, jadi gak bisa ngejalanin perintah
Jawaban Anda [a-e]: a
❌ Salah. Jawaban benar: c
🧾 Penjelasan: Karena belum ada JavaScript yang menangani aksi tombol...
```

---

## 💬 Butuh Bantuan?

Kalau kamu punya pertanyaan, ide pengembangan, atau ketemu bug, langsung aja:
- 📧 Chat/email ke kami
- 🐛 Atau buat [Issue](https://github.com/supportpineaplehub/LenrJsPine/issues) di GitHub

Selamat belajar & semangat terus! 🍍💻