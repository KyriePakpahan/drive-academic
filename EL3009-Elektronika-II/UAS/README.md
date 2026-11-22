# EL3009 Elektronika II · Paket Persiapan UAS (ITB)

Repositori terstruktur untuk persiapan **Ujian Akhir Semester (Ujian 2) EL3009 Elektronika II**, Teknik Elektro ITB. Seluruh dokumen disusun mengikuti kisi-kisi resmi **pekan 9—15** (DC-DC Converter, Building Block IC, Differential Amplifier, Multistage Amplifier, dan Operational Amplifier CMOS) dengan buku acuan **Adel S. Sedra & Kenneth C. Smith Ed. 7** dan **Daniel W. Hart (*Power Electronics*)**. Seluruh perhitungan telah diverifikasi secara simbolik dan numerik menggunakan Python (`SymPy`/`NumPy`), dilengkapi skematik rangkaian **LaTeX CircuiTikZ** serta plot gelombang 300 DPI, dan tersedia dalam format **`.docx` native (persamaan OMML editable, terverifikasi WordCraft CLI v0.18.1 `--strict`)** beserta **`.pdf` pendamping**.

---

## Peta Urutan Belajar (*Study Roadmap*)

Ikuti 3 tahap di bawah ini secara berurutan agar tidak ada celah pemahaman (*zero knowledge gap*) saat menghadapi Ujian 2 tutup buku (hanya kalkulator saintifik, durasi 150 menit):

### Tahap 1: Kuasai Fondasi Materi Sesuai Kisi-Kisi (`01-materi-uas/`)

| Urutan | Cakupan Kisi-Kisi Ujian 2 (Pekan 9—15) | Dokumen `.docx` | Versi `.pdf` |
|---:|---|---|---|
| 0 | Prasyarat Fondasi: Model DC & Sinyal Kecil MOSFET, Degenerasi *Source*, *Volt-Second* & *Charge Balance* | [Modul 00 (.docx)](01-materi-uas/Modul-00_Prasyarat-Fondasi_Model-MOSFET-dan-Konverter-Daya.docx) | [PDF](01-materi-uas/Modul-00_Prasyarat-Fondasi_Model-MOSFET-dan-Konverter-Daya.pdf) |
| 1 | Topik 1 · DC-DC Converter (*Buck*, *Boost*, *Buck-Boost*, CCM/BCM, *Worst-Case* $D$, GaN & ESR) | [Modul 01 (.docx)](01-materi-uas/Modul-01_Topik-1_DC-DC-Converter_Buck-Boost-dan-Buck-Boost.docx) | [PDF](01-materi-uas/Modul-01_Topik-1_DC-DC-Converter_Buck-Boost-dan-Buck-Boost.pdf) |
| 2 | Topik 2 · Building Block IC (*Current Mirror*, Degenerasi $R_S$, *Cascode*, *Wide-Swing*, *Current Steering*, CS Aktif) | [Modul 02 (.docx)](01-materi-uas/Modul-02_Topik-2_Building-Block-IC_Current-Mirror-Steering-dan-Cascode.docx) | [PDF](01-materi-uas/Modul-02_Topik-2_Building-Block-IC_Current-Mirror-Steering-dan-Cascode.pdf) |
| 3 | Topik 3 · Differential Amplifier (Beban Resistor & Beban Aktif, *Half-Circuit*, *Mismatch* CMRR, Rentang $V_{CM}$ & $v_O$) | [Modul 03 (.docx)](01-materi-uas/Modul-03_Topik-3_Differential-Amplifier_Beban-Resistor-dan-Aktif.docx) | [PDF](01-materi-uas/Modul-03_Topik-3_Differential-Amplifier_Beban-Resistor-dan-Aktif.pdf) |
| 4 | Topik 4 · Multistage Amplifier (*Interstage Loading*, *Direct Coupling*, Efek Miller, *Pole Splitting*, & $R_z$) | [Modul 04 (.docx)](01-materi-uas/Modul-04_Topik-4_Multistage-Amplifier_Interstage-Loading-dan-Kompensasi.docx) | [PDF](01-materi-uas/Modul-04_Topik-4_Multistage-Amplifier_Interstage-Loading-dan-Kompensasi.pdf) |
| 5 | Topik 5 · Operational Amplifier CMOS (*Two-Stage* & *Folded-Cascode*, Bias DC, $A_v$, CMRR, $f_t$, $f_P$, *Slew Rate*) | [Modul 05 (.docx)](01-materi-uas/Modul-05_Topik-5_Operational-Amplifier-CMOS_Two-Stage-dan-Folded-Cascode.docx) | [PDF](01-materi-uas/Modul-05_Topik-5_Operational-Amplifier-CMOS_Two-Stage-dan-Folded-Cascode.pdf) |

### Tahap 2: Latihan Mandiri Menggunakan Bank Soal Terverifikasi (`02-bank-soal-dan-pembahasan/`)

Setiap dokumen dipisahkan tegas dengan jeda halaman antara **Bagian I (Naskah Soal Bersih tanpa bocoran)** dan **Bagian II (Pembahasan Langkah demi Langkah Terverifikasi SymPy + Kotak Audit Koreksi Arsip Mahasiswa)**.

| Bundel | Cakupan Paket Soal | Dokumen `.docx` | Versi `.pdf` |
|---|---|---|---|
| **Bank Soal 01** | UAS Resmi 2024 (31 Des 2024) & Ujian 2 2025 (100% Fokus Kisi-Kisi + Audit Jawaban Mahasiswa) | [Bank Soal 01 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-01_UAS-EL3009_2024-dan-2025_Fokus-Kisi-Kisi.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-01_UAS-EL3009_2024-dan-2025_Fokus-Kisi-Kisi.pdf) |
| **Bank Soal 02** | Soal Kisi-Kisi Arsip 2021—2022: UAS 2021 (#1—3), UTS 2022 (#1—2), & HME 2022 (#4 *Buck-Boost* + Audit) | [Bank Soal 02 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-02_Arsip-Kisi-Kisi_UAS-2021_UTS-2022_dan_HME-Buck-Boost.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-02_Arsip-Kisi-Kisi_UAS-2021_UTS-2022_dan_HME-Buck-Boost.pdf) |
| **Bank Soal 03** | Kurasi PR Pekan 9—15 (`PR-05`, `PR-07`, `PR-08`, `PR-09`, `PR-11`, `PR-12`, `PR-07 2026`) & `Kuis 4 2025` + Audit Koreksi | [Bank Soal 03 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-03_Kurasi-PR-Pekan-9-15_dan_Kuis-4-EL3009.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-03_Kurasi-PR-Pekan-9-15_dan_Kuis-4-EL3009.pdf) |
| **Bank Soal 04 (Lampiran)** | **Di Luar Kisi-Kisi Ujian 2:** *Feedback Amplifier* (UAS 21 #4, UTS 22 #3) & HME 2022 #1—3 (*Oscillator*, *SigGen*, *Butterworth* + Audit) | [Bank Soal 04 (.docx)](02-bank-soal-dan-pembahasan/Bank-Soal-04_Lampiran_Di-Luar-Kisi-Kisi-Ujian-2.docx) | [PDF](02-bank-soal-dan-pembahasan/Bank-Soal-04_Lampiran_Di-Luar-Kisi-Kisi-Ujian-2.pdf) |

### Tahap 3: Pemantapan Tutup Buku & Simulasi Akhir (`03-latihan-dan-ringkasan/`)

| Dokumen | Fokus Utama | Dokumen `.docx` | Versi `.pdf` |
|---|---|---|---|
| ***Cheat Sheet* & Strategi Ujian 2** | **Bagian A:** Lembar rumus inti siap cetak **2 halaman A4 bolak-balik**; **Bagian B:** Manajemen waktu 150 menit, trik kalkulator, & **10 Jebakan Klasik Ujian 2 EL3009** | [*Cheat Sheet* (.docx)](03-latihan-dan-ringkasan/Cheat-Sheet_dan_Strategi-Ujian-2_EL3009.docx) | [PDF](03-latihan-dan-ringkasan/Cheat-Sheet_dan_Strategi-Ujian-2_EL3009.pdf) |
| **Simulasi Prediksi Ujian 2 (2026/2027)** | 5 soal sintesis orisinal mode 150 menit mencakup seluruh 5 topik (termasuk *Multistage* + kompensasi Miller & *Folded-Cascode*) + kunci terverifikasi & rubrik 100 poin | [Simulasi Ujian 2 (.docx)](03-latihan-dan-ringkasan/Simulasi-Prediksi-Ujian-2_EL3009_2026-2027.docx) | [PDF](03-latihan-dan-ringkasan/Simulasi-Prediksi-Ujian-2_EL3009_2026-2027.pdf) |

### Arsip Mentah Sumber (`00-arsip-mentah/`)

Seluruh berkas sumber asli (kisi-kisi pekan 9—15, 4 PDF soal UAS/UTS 2021—2025, 8 PDF arsip HME 2022, serta 9 berkas PR pekan 9—15 dan Kuis 4) tersimpan rapi dan terdeduplikasi di [`00-arsip-mentah/`](00-arsip-mentah/README.md).
