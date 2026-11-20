# EL3010 Pengolahan Sinyal Digital · Paket Persiapan UAS (ITB)

Repositori terstruktur untuk persiapan **Ujian Akhir Semester (UAS) EL3010 Pengolahan Sinyal Digital (PSD)**, Teknik Elektro ITB. Seluruh dokumen disusun mengikuti **silabus resmi `Rencana Kuliah Sem. 1-2026/2027`** dengan buku acuan Proakis & Manolakis Ed. 4 (`[PrMa07]`), seluruh perhitungan telah diverifikasi secara simbolik dan numerik, serta tersedia dalam format **`.docx` (terverifikasi WordCraft v0.18.1)** dan **`.pdf` pendamping** agar mudah dibaca langsung di GitHub, tablet, maupun ponsel.

---

## Peta Urutan Belajar (*Study Roadmap*)

Ikuti 5 tahap di bawah ini secara berurutan agar tidak ada celah pemahaman saat menghadapi soal ujian tutup buku (hanya kalkulator saintifik):

### Tahap 1: Kuasai Fondasi Materi Sesuai Silabus (`01-materi-uas/`)

| Urutan | Cakupan Silabus (`[PrMa07]`) | Dokumen `.docx` | Versi `.pdf` |
|---:|---|---|---|
| 0 | Prasyarat Pra-UTS: Transformasi-z, ROC, PFE, ZIR/ZSR Satu Sisi, DTFT & Parseval (Bab 3–4) | [Modul 00 (.docx)](01-materi-uas/Modul-00_Prasyarat-Pra-UTS_Transformasi-Z_dan_DTFT.docx) | [PDF](01-materi-uas/Modul-00_Prasyarat-Pra-UTS_Transformasi-Z_dan_DTFT.pdf) |
| 1 | Mg 9–10 · Karakteristik Sistem LTI Domain Frekuensi & Filter Selektif (Bab 5: 5.1–5.4) | [Modul 01 (.docx)](01-materi-uas/Modul-01_Mg09-10_Bab5_Respons-Frekuensi-LTI_dan_Filter-Selektif.docx) | [PDF](01-materi-uas/Modul-01_Mg09-10_Bab5_Respons-Frekuensi-LTI_dan_Filter-Selektif.pdf) |
| 2 | Mg 11 · DFT, Sifat DFT, Pentapisan Linier (*Overlap-Add/Save*), Analisis Frekuensi (Bab 7: 7.1–7.4) | [Modul 02 (.docx)](01-materi-uas/Modul-02_Mg11_Bab7_DFT_Pentapisan-Linier_dan_Analisis-Frekuensi.docx) | [PDF](01-materi-uas/Modul-02_Mg11_Bab7_DFT_Pentapisan-Linier_dan_Analisis-Frekuensi.pdf) |
| 3 | Mg 12 · *Fast Fourier Transform* (FFT Radix-2 DIT & DIF, *Butterfly*, IFFT) (Bab 8: 8.1–8.2) | [Modul 03 (.docx)](01-materi-uas/Modul-03_Mg12_Bab8_Fast-Fourier-Transform-FFT.docx) | [PDF](01-materi-uas/Modul-03_Mg12_Bab8_Fast-Fourier-Transform-FFT.pdf) |
| 4 | Mg 13 · Struktur dan Implementasi Filter FIR & IIR (DF-I, DF-II, Kaskade, Paralel) (Bab 9: 9.1–9.3) | [Modul 04 (.docx)](01-materi-uas/Modul-04_Mg13_Bab9_Struktur-dan-Implementasi-Filter.docx) | [PDF](01-materi-uas/Modul-04_Mg13_Bab9_Struktur-dan-Implementasi-Filter.pdf) |
| 5 | Mg 14–15 · Desain Filter Digital (FIR *Windowing*/*Freq. Sampling*, IIR *Bilinear*, Transformasi Frekuensi) (Bab 10: 10.1–10.4) | [Modul 05 (.docx)](01-materi-uas/Modul-05_Mg14-15_Bab10_Desain-Filter-Digital_FIR_IIR_dan_Transformasi.docx) | [PDF](01-materi-uas/Modul-05_Mg14-15_Bab10_Desain-Filter-Digital_FIR_IIR_dan_Transformasi.pdf) |

### Tahap 2: Latihan Mandiri Menggunakan Bank Soal Asli (`02-bank-soal-dan-pembahasan/`)

Setiap dokumen dipisahkan tegas menjadi **Bagian I (Naskah Soal Bersih tanpa bocoran)** dan **Bagian II (Pembahasan Langkah demi Langkah + Audit Koreksi Arsip Lama)**.

| Bundel | Cakupan Paket Ujian | Dokumen `.docx` | Versi `.pdf` |
|---|---|---|---|
| **Bank Soal 01** | UAS Resmi 2020/2021, 2021/2022, dan 2022/2023 + Kotak Audit Koreksi Solusi Arsip HME | [Bank Soal 01 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-01_UAS-EL3010_2020-2023.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-01_UAS-EL3010_2020-2023.pdf) |
| **Bank Soal 02** | UAS Resmi Terbaru 2024/2025 & 2025/2026 (6 Problem lengkap perdana, teks soal Inggris organik) | [Bank Soal 02 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-02_UAS-EL3010_2024-2026.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-02_UAS-EL3010_2024-2026.pdf) |
| **Bank Soal 03** | Ekstraksi 28 Halaman Bundel Post Test 2016–2018 (PT3 2017, PT3 2018, PT4 2016, PT4 2017, PT5 2016) + Audit 13 Salah Cetak Buku | [Bank Soal 03 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-03_Bundel-Post-Test-2016-2018.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-03_Bundel-Post-Test-2016-2018.pdf) |

### Tahap 3: Pemantapan Tutup Buku & Simulasi Akhir (`03-latihan-dan-ringkasan/`)

| Dokumen | Fokus Utama | Dokumen `.docx` | Versi `.pdf` |
|---|---|---|---|
| **Cheat Sheet & Strategi UAS** | Peta rumus inti Bab 3–10, *decision tree* metode, trik kalkulator saintifik, dan **10 Jebakan Klasik UAS EL3010** | [Cheat Sheet (.docx)](03-latihan-dan-ringkasan/Cheat-Sheet_dan_Strategi-UAS-Tutup-Buku_EL3010.docx) | [PDF](03-latihan-dan-ringkasan/Cheat-Sheet_dan_Strategi-UAS-Tutup-Buku_EL3010.pdf) |
| **Simulasi Prediksi UAS 2026/2027** | 3 soal sintesis baru mode ujian 120 menit (DF-II + ZIR/ZSR, Radix-2 FFT + Overlap-Add, FIR Hanning + IIR Bilinear & HPF) + kunci dan rubrik 100 poin | [Simulasi UAS (.docx)](03-latihan-dan-ringkasan/Simulasi-Prediksi-UAS_EL3010_2026-2027.docx) | [PDF](03-latihan-dan-ringkasan/Simulasi-Prediksi-UAS_EL3010_2026-2027.pdf) |

### Arsip Mentah Sumber (`00-arsip-mentah/`)

Seluruh file sumber asli (silabus, 7 PDF soal UAS resmi terdeduplikasi, 6 PDF solusi arsip HME, serta 28 foto berurutan hal. 170–197 beserta PDF gabungannya) tersimpan rapi di [`00-arsip-mentah/`](00-arsip-mentah/README.md).
