# EL3009 Elektronika II · Paket Persiapan UAS (ITB · Edisi v3 Buku Teks Naratif)

Repositori terstruktur untuk persiapan **Ujian Akhir Semester (Ujian 2) EL3009 Elektronika II**, Teknik Elektro ITB. Seluruh **12 dokumen (170 halaman, 43.689 kata, 0 halaman kosong)** difokuskan **100% pada 5 topik resmi kisi-kisi pekan 9 sampai 15** (*DC-DC Converter*, *Building Block IC*, *Differential Amplifier*, *Multistage Amplifier*, dan *Operational Amplifier* CMOS/$\mu\text{A}741$) dengan sintesis naratif penuh dari buku acuan **Adel S. Sedra & Kenneth C. Smith Ed. 7/8**, **Behzad Razavi**, **Daniel W. Hart (*Power Electronics*)**, serta **Erickson & Maksimović**.

**Pembaruan Besar Edisi v3:**
- **Buku Teks Naratif Penuh (CMOS + BJT Paralel):** Seluruh 6 modul diperdalam 2,5 kali sampai 3 kali lipat dengan penurunan fisis langkah demi langkah (tanpa celah pengetahuan), meliputi non-idealitas *DC-DC Converter* ($R_{\text{sw}}, r_L$, ESR, *Synchronous*, DCM), BJT paralel (*Wilson*, *Widlar*, *Diff Pair* $\tanh$, $\mu\text{A}741$), *Common-Gate* + *Body Effect*, *Current-Mirror Doublet* & OTA 3 cermin, *Class A/B/AB*, OCTC, penurunan KCL 2-*node* Miller + $R_z$, hingga komplemen input PMOS & *Rail-to-Rail* *Folded-Cascode*.
- **Pembahasan Penuntun Gaya Bundel + 18 Kotak Audit Koreksi SymPy:** Seluruh 4 Bank Soal dan Simulasi ditulis ulang dengan gaya penuntun 5 lapis (memetakan diketahui, menuntun alur berpikir, menurunkan langkah per langkah, verifikasi fisis, serta mengoreksi kekeliruan nyata pada kunci resmi Kuis 4 2025, PR-05 sampai PR-12 2024, PR-07 2025, PR-06 2026, HME #4, dan Bundel UTS 2017 #3B).
- **100% Bersih Topik UAS & Bundel 2018/2019 Dirapikan:** Seluruh materi di luar kisi-kisi UAS (*Feedback*, *Oscillator*, *Pembangkit Sinyal*, *Filter Butterworth*, HME #1 sampai #3) telah dihapus tuntas. Arsip pindaian mentah `20261123.pdf` (145,2 MB) telah dideduplikasi, diurutkan (`hal. 54` sampai `123`), dikompresi tajam menjadi 5 PDF bersih (`7,04 MB`), dan soal terbaiknya dikurasi ke **Bank Soal 04** baru.
- **50 Visual 300 DPI + 7.163 Persamaan Native WordCraft (`--strict` PASS):** 41 skematik LaTeX CircuiTikZ monokrom standar Sedra & Smith (panah *Source* keluar = NMOS, masuk = PMOS, beserta BJT NPN/PNP) dan 9 grafik fisika Matplotlib 300 DPI. Seluruh **7.163 persamaan** di 12 berkas `.docx` disusun langsung melalui `wordcraft-cli v0.18.1` (`insert.equation` & `equation.number`) dan lolos `wordcraft-cli convert --update-fields --strict`.

---

## Peta Urutan Belajar (*Study Roadmap*)

Ikuti 3 tahap di bawah ini secara berurutan agar tidak ada celah pemahaman saat menghadapi Ujian 2 tutup buku (hanya kalkulator saintifik, durasi 150 menit):

### Tahap 1: Kuasai Buku Teks Naratif Sesuai Kisi-Kisi (`01-materi-uas/`)

| Urutan | Cakupan Kisi-Kisi Ujian 2 (Pekan 9 sampai 15) | Hal. / Kata / Pers. WC | Dokumen `.docx` | Versi `.pdf` |
|---:|---|---:|---|---|
| 0 | Prasyarat Fondasi: Fisika & Model Sinyal Kecil MOSFET + BJT Paralel, Degenerasi $R_S/R_E$, *Volt-Second* & *Charge Balance* | 20 hal · 6.292 kata · 751 eq | [Modul 00 (.docx)](01-materi-uas/Modul-00_Prasyarat-Fondasi_Model-MOSFET-dan-Konverter-Daya.docx) | [PDF](01-materi-uas/Modul-00_Prasyarat-Fondasi_Model-MOSFET-dan-Konverter-Daya.pdf) |
| 1 | Topik 1 · DC-DC Converter (*Buck*, *Boost*, *Buck-Boost*, Non-Ideal $R_{\text{sw}}/r_L$/ESR, *Synchronous*, CCM/BCM/DCM, *Worst-Case* $D^* = 1/3$, GaN) | 22 hal · 5.563 kata · 853 eq | [Modul 01 (.docx)](01-materi-uas/Modul-01_Topik-1_DC-DC-Converter_Buck-Boost-dan-Buck-Boost.docx) | [PDF](01-materi-uas/Modul-01_Topik-1_DC-DC-Converter_Buck-Boost-dan-Buck-Boost.pdf) |
| 2 | Topik 2 · Building Block IC (MOSFET & BJT *Mirrors*: *Basic*, $R_S$, *Cascode*, *Wide-Swing*, *Wilson*, *Widlar*, *Steering*, CG + *Body Effect*, *Telescopic*/*Folded*, *Darlington*) | 17 hal · 4.978 kata · 735 eq | [Modul 02 (.docx)](01-materi-uas/Modul-02_Topik-2_Building-Block-IC_Current-Mirror-Steering-dan-Cascode.docx) | [PDF](01-materi-uas/Modul-02_Topik-2_Building-Block-IC_Current-Mirror-Steering-dan-Cascode.pdf) |
| 3 | Topik 3 · Differential Amplifier (MOSFET & BJT Paralel, ICMR, Sinyal Besar $\sqrt{2}V_{OV}$ vs $\tanh$, *Half-Circuit*, $R_S/R_e$, *Cascode*, *Mismatch* & *Offset*, Beban Aktif + *Doublet*, OTA 3 Cermin) | 17 hal · 4.395 kata · 636 eq | [Modul 03 (.docx)](01-materi-uas/Modul-03_Topik-3_Differential-Amplifier_Beban-Resistor-dan-Aktif.docx) | [PDF](01-materi-uas/Modul-03_Topik-3_Differential-Amplifier_Beban-Resistor-dan-Aktif.pdf) |
| 4 | Topik 4 · Multistage Amplifier (*Direct Coupling*, *Interstage Loading*, *Class A/B/AB*, Kapasitansi HF & $f_T$, OCTC, KCL 2-*Node* Miller, *Pole Splitting*, & 3 Opsi $R_z$) | 15 hal · 4.254 kata · 546 eq | [Modul 04 (.docx)](01-materi-uas/Modul-04_Topik-4_Multistage-Amplifier_Interstage-Loading-dan-Kompensasi.docx) | [PDF](01-materi-uas/Modul-04_Topik-4_Multistage-Amplifier_Interstage-Loading-dan-Kompensasi.pdf) |
| 5 | Topik 5 · Operational Amplifier CMOS (*Two-Stage*, *Folded-Cascode* + Komplemen Input PMOS & *Rail-to-Rail*, PSRR, *Slew Rate*, & Pembanding BJT $\mu\text{A}741$) | 18 hal · 4.740 kata · 854 eq | [Modul 05 (.docx)](01-materi-uas/Modul-05_Topik-5_Operational-Amplifier-CMOS_Two-Stage-dan-Folded-Cascode.docx) | [PDF](01-materi-uas/Modul-05_Topik-5_Operational-Amplifier-CMOS_Two-Stage-dan-Folded-Cascode.pdf) |

### Tahap 2: Latihan Mandiri Menggunakan Bank Soal Gaya Penuntun (`02-bank-soal-dan-pembahasan/`)

Setiap dokumen dipisahkan tegas dengan jeda halaman antara **Bagian I (Naskah Soal Bersih tanpa bocoran rumus pada gambar maupun teks)** dan **Bagian II (Pembahasan Penuntun Gaya Bundel 5 Lapis Terverifikasi SymPy + Kotak Audit Koreksi)**.

| Bundel | Cakupan Paket Soal (100% Kisi-Kisi UAS) | Hal. / Kata / Pers. WC | Dokumen `.docx` | Versi `.pdf` |
|---|---|---:|---|---|
| **Bank Soal 01** | UAS Resmi 2024 (31 Des 2024, SPDT 2 posisi) & Ujian 2 2025 (100% Fokus Kisi-Kisi + 5 Kotak Audit Jawaban Mahasiswa) | 18 hal · 3.714 kata · 761 eq | [Bank Soal 01 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-01_UAS-EL3009_2024-dan-2025_Fokus-Kisi-Kisi.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-01_UAS-EL3009_2024-dan-2025_Fokus-Kisi-Kisi.pdf) |
| **Bank Soal 02** | Soal Kisi-Kisi Arsip 2021 sampai 2022: UAS 2021 (#1 sampai #3), UTS 2022 (#1 sampai #2), & HME 2022 (#4 *Buck-Boost* + Audit) | 10 hal · 2.023 kata · 445 eq | [Bank Soal 02 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-02_Arsip-Kisi-Kisi_UAS-2021_UTS-2022_dan_HME-Buck-Boost.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-02_Arsip-Kisi-Kisi_UAS-2021_UTS-2022_dan_HME-Buck-Boost.pdf) |
| **Bank Soal 03** | 13 Latihan Kurasi PR Pekan 9 sampai 15 (`PR-05` sampai `PR-12` 2024, `Kuis 4 2025`, `PR-06` sampai `PR-11` 2025, `PR-06` sampai `PR-08` 2026) + 10 Kotak Audit | 13 hal · 3.188 kata · 699 eq | [Bank Soal 03 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-03_Kurasi-PR-Pekan-9-15_dan_Kuis-4-EL3009.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-03_Kurasi-PR-Pekan-9-15_dan_Kuis-4-EL3009.pdf) |
| **Bank Soal 04 (Baru)** | Kurasi 6 Paket Soal Terbaik **Bundel Elektroteknik 2018/2019** (`hal. 54` sampai `123`, UTS 2017 & Ujian 2018: DC-DC, *Cascode*/CG, Diff Amp CMOS/BJT, Miller KCL, *Two-Stage*, & *Folded-Cascode* 80 dB) | 9 hal · 2.040 kata · 366 eq | [Bank Soal 04 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-04_Bundel-Elektroteknik-2018_Fokus-5-Topik-UAS.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-04_Bundel-Elektroteknik-2018_Fokus-5-Topik-UAS.pdf) |

### Tahap 3: Pemantapan Tutup Buku & Simulasi Akhir (`03-latihan-dan-ringkasan/`)

| Dokumen | Fokus Utama | Hal. / Kata / Pers. WC | Dokumen `.docx` | Versi `.pdf` |
|---|---|---:|---|---|
| ***Cheat Sheet* & Strategi Ujian 2** | **Bagian A:** Lembar rumus inti siap cetak **tepat 2 halaman A4 bolak-balik** (CMOS + BJT + DC-DC + $\mu\text{A}741$); **Bagian B:** Manajemen waktu 150 menit, trik kalkulator, & **10 Jebakan Klasik UAS (Hasil Audit 2017 sampai 2026)** | 3 hal · 1.073 kata · 263 eq | [*Cheat Sheet* (.docx)](03-latihan-dan-ringkasan/Cheat-Sheet_dan_Strategi-Ujian-2_EL3009.docx) | [PDF](03-latihan-dan-ringkasan/Cheat-Sheet_dan_Strategi-Ujian-2_EL3009.pdf) |
| **Simulasi Prediksi Ujian 2 (2026/2027)** | 5 soal sintesis orisinal mode 150 menit bebas bocoran (mencakup seluruh 5 topik termasuk *Multistage* + kompensasi Miller & *Folded-Cascode*) + pembahasan penuntun gaya Bundel & rubrik 100 poin | 8 hal · 1.429 kata · 254 eq | [Simulasi Ujian 2 (.docx)](03-latihan-dan-ringkasan/Simulasi-Prediksi-Ujian-2_EL3009_2026-2027.docx) | [PDF](03-latihan-dan-ringkasan/Simulasi-Prediksi-Ujian-2_EL3009_2026-2027.pdf) |

### Arsip Mentah Sumber (`00-arsip-mentah/`)

Seluruh berkas sumber asli 100% fokus kisi-kisi UAS (kisi-kisi pekan 9 sampai 15, 4 PDF soal UAS/UTS 2021 sampai 2025, 2 PDF HME 2022 Soal 4 *Buck-Boost*, 20 berkas PR 2024 sampai 2026 & Kuis 4 2025, serta **5 PDF rapi Bundel Elektroteknik 2018/2019** hasil deduplikasi & kompresi dari pindaian mentah 145,2 MB menjadi 7,04 MB) tersimpan terstruktur di [`00-arsip-mentah/`](00-arsip-mentah/README.md). Buku teks berhak cipta (Sedra & Smith, Hart) dan slide kuliah dosen tidak diunggah ke repositori publik ini.
