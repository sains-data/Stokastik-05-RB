# 📊 Analisis Transisi Kategori Indeks Prestasi (IP) Mahasiswa  
**Model Rantai Markov Waktu-Diskrit (DTMC)**  
*Studi Kasus: Mahasiswa Sains Data ITERA Angkatan 2022 (Semester 1–6)*

## 🧠 Gambaran Umum
Repository ini berisi analisis stokastik menggunakan **Discrete-Time Markov Chain (DTMC)** untuk memodelkan **pola perpindahan kategori Indeks Prestasi (IP)** mahasiswa antar semester.  

Yang dianalisis pada proyek ini:  
- ✅ Matriks **Probabilitas Transisi 1-Langkah**
- ✅ **Peluang Transisi n-Langkah** (2-Step & 3-Step)
- ✅ **Distribusi Stasioner (Steady-State)**
- ✅ **Validasi Monte Carlo**
- ✅ **Mean First Passage Time (MFPT)**
- ✅ Insight perkembangan akademik mahasiswa

## 🏷️ Definisi State (Kategori IP)
| **State** | **Interval IP** | **Kategori** |
|--------|----------------|-------------|
| A | 3.26 – 4.00 | Sangat Baik |
| B | 2.76 – 3.25 | Baik |
| C | 2.01 – 2.75 | Cukup |
| D | 1.01 – 2.00 | Kurang |
| E | 0.00 – 1.00 | Sangat Kurang |

> ⚠️ State **E dieliminasi**, sehingga model menggunakan **4×4 State-Space**

## 📌 Hasil Utama
### 🔹 Distribusi Steady-State (Jangka Panjang)

π = [0.542, 0.304, 0.135, 0.020]

### 🔹 Perkiraan Distribusi Mahasiswa dalam Jangka Panjang (Total 103)
| State | Perkiraan Jumlah |
|-------|----------------|
| A | 56 Mahasiswa |
| B | 31 Mahasiswa |
| C | 14 Mahasiswa |
| D | 2 Mahasiswa |

### 🔹 Validasi Monte Carlo (Semester 7 & 8)
Hasil **mendekati perhitungan analitik**, menandakan model mampu menangkap pola transisi cukup baik.

## 🛠️ Teknologi yang Digunakan
- `R`
- `RMarkdown (.Rmd / .Rmd)`
- `Matrix operations`
- `Data Visualization (ggplot2 / base R)`
- `Monte Carlo Simulation`

## 📁 Struktur Repository

├── data/
│   └── Dataset_5_RB.csv
├── report/
│   └── Code_5_RB.Rmd
├── analysis/
│   └── Laporan_5_RB.pdf
├── video/
│   └── Video_5_RB.mp4
├── poster/
│   └── Poster_5_RB.pdf
└── README.md

## 🫅 Kontributor

| **Nama**                      | **NIM**   |
| ----------------------------- | --------- |
| Eksanty F Sugma Islamiaty | 122450001 |
| Arafi Ramadhan Maulana        | 122450002 |
| Kayla Amanda Sukma            | 122450086 |
| Aditya Rahman                 | 122450113 |

## ⭐ Jika repository ini bermanfaat, beri STAR ya! 🚀
Terbuka untuk diskusi dan kolaborasi penelitian di bidang stokastik dan analisis akademik mahasiswa.
