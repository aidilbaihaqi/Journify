# FINAL PROJECT PEMROGRAMAN PERANGKAT MOBILE APLIKASI JOURNALING UNTUK DETEKSI MOOD DENGAN ANALISIS SENTIMEN BERBASIS ANDROID FLUTTER

## Fitur Frontend (Flutter - MVVM)
<ol>
  <li>Login/Register (pakai provider dan http)</li>
  <li>Home Page (greeting + tombol journaling)</li>
  <li>Text Journaling + kirim ke backend (POST api/journal)</li>
  <li>Speech-to-Text Journaling + kirim ke backend (POST api/journal)</li>
  <li>Riwayat Jurnal (tampilkan di dashboard user) (GET api/history)</li>
  <li>Analisis Sentimen (tampilkan hasil + mood)</li>
  <li>Profil & Statistik</li>
<ol>

## Fitur Backend (Django REST Framework)
<ol>
  <li>User Authentication (login/register)</li>
  <li>Menyimpan & mengambil data jurnal</li>
  <li>Mengolah sentimen (via NLP atau API Eksternal)</li>
  <li>Memberikan hasil mood ke frontend flutter</li>
</ol>

## Cara Frontend dan Backend berkomunikasi
```bash
[Flutter App]
  ↓ POST /api/journals/
[ Django Backend ]
  → Simpan jurnal → Analisis Sentimen → Return { "mood": "Bahagia" }
```

