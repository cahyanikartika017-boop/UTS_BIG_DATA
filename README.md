# Analisis Sentimen Aplikasi JMO (Jamsostek Mobile)

Repository ini dibuat untuk memenuhi tugas **UTS Big Data**.  
Berisi hasil scraping dan analisis sentimen dari ulasan pengguna aplikasi **JMO** di Google Play Store.

## 🎯 Objek Analisis
**Aplikasi:** JMO (Jamsostek Mobile)  
**Pengembang:** BPJS Ketenagakerjaan (Badan Penyelenggara Jaminan Sosial Ketenagakerjaan)  
**Fungsi:** Layanan digital kepesertaan, klaim JHT, cek saldo, dan informasi ketenagakerjaan lainnya.  

## 👤 Identitas
- **Nama:** Kartika Cahyani  
- **NIM:** 14022300049  

## 📁 Isi Repository
- `scraping.ipynb` - Notebook untuk scraping ulasan dari Google Play Store.
- `sentiment_analysis.ipynb` - Notebook untuk analisis sentimen menggunakan model Hugging Face.
- `ulasan_google_play.csv` - Dataset hasil scraping (100+ ulasan terbaru).
- `README.md` - Penjelasan proyek ini.

## 🛠️ Tools & Library yang Digunakan
| Keperluan | Tools / Library |
|-----------|----------------|
| Scraping | `google-play-scraper` |
| Analisis Sentimen | `transformers` (Hugging Face) dengan model `w11wo/indonesian-roberta-base-sentiment-classifier` |
| Pengolahan Data | `pandas`, `numpy` |
| Visualisasi | `matplotlib`, `seaborn` (opsional) |

## 📊 Hasil yang Diharapkan
- Mendapatkan label sentimen (POSITIVE / NEGATIVE) dari setiap ulasan.
- Mengetahui persentase kepuasan pengguna terhadap aplikasi JMO.
- Menemukan keluhan umum atau pujian yang sering disebut pengguna.

## 🔗 Sumber Data
Ulasan diambil dari Google Play Store:  
[https://play.google.com/store/apps/details?id=com.bpjstku](https://play.google.com/store/apps/details?id=com.bpjstku)

## 🚀 Cara Menjalankan
1. Clone repository ini ke lokal atau buka di Google Colab.
2. Install library yang dibutuhkan:
   ```bash
   pip install google-play-scraper pandas transformers torch
