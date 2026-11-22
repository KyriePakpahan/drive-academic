# Arsip Mentah UAS EL3009 Elektronika II

Folder ini menyimpan seluruh berkas sumber asli dari dua folder Google Drive ujian, kisi-kisi resmi Ujian 2 pekan 9—15, serta koleksi PR pekan 9—15 dan Kuis 4 dari Google Drive EL3009. Seluruh berkas telah dideduplikasi berdasarkan checksum SHA-256 dan diberi nama secara konsisten.

## Ringkasan Isi

1. **`kisi-kisi/`** (1 berkas)
   - `Kisi-Kisi_Ujian-2_EL3009_Pekan-9-15.png`: daftar resmi 5 topik Ujian 2 (DC-DC Converter, Building Block, Differential Amplifier, Multistage Amplifier, dan Operational Amplifier).
2. **`soal-uas-resmi/`** (4 PDF unik)
   - `EL3009_UAS_2021_Soal-1-4.pdf`: 4 soal (Cascode Amplifier, Penguat Diferensial beban aktif, CMOS Op-Amp 2-tingkat, dan *Feedback Amplifier*).
   - `EL3009_UTS_2022-2023_Soal-1-3_Arsip-Folder-UAS.pdf`: tajuk asli lembar soal adalah **Ujian Tengah Semester EL3009 Elektronika II, Semester I 2022/2023 (13 Oktober 2022)** yang tersimpan di folder UAS Drive. Soal 1 (*Current Mirror* degenerasi $R_S$) dan Soal 2 (*Differential Amplifier*) relevan dengan kisi-kisi Ujian 2, sedangkan Soal 3 (*Feedback Amplifier*) ditempatkan di lampiran.
   - `EL3009_UAS_2024_Soal-1-4.pdf`: UAS resmi 31 Desember 2024 (tutup buku, 150 menit) berisi 4 soal yang sepenuhnya sesuai kisi-kisi Ujian 2 (*Boost Converter*, Blok Pembangun IC, Penguat Diferensial beban aktif, dan Op-Amp *Folded-Cascode*).
   - `EL3009_Ujian-2_2025_Soal-1-4_dan_Jawaban-Mahasiswa.pdf`: lembar Ujian 2 beserta jawaban tulis tangan mahasiswa untuk keempat soal kisi-kisi.
3. **`arsip-hme-2022/`** (8 PDF: 4 soal + 4 jawaban mahasiswa NIM `13219031`)
   - `HME-2022_Soal-4_DC-DC-Converter.pdf` (*Buck-Boost Converter*) sesuai kisi-kisi Ujian 2 dan dibahas pada Bank Soal 02.
   - `HME-2022_Soal-1_Oscillator.pdf`, `HME-2022_Soal-2_Pembangkit-Sinyal.pdf`, dan `HME-2022_Soal-3_Filter-Butterworth.pdf` merupakan topik kurikulum lama di luar kisi-kisi Ujian 2 sehingga dipisahkan ke Bank Soal 04 (Lampiran).
   - **Catatan Audit:** Jawaban tulis tangan pada arsip ini memuat beberapa kekeliruan teknis (antara lain kesalahan rumus frekuensi sebesar faktor 10 pada Soal 2 serta salah tulis satuan $\mu\text{F}$ alih-alih $\mu\text{H}$ pada Soal 4). Gunakan pembahasan terverifikasi di `../02-bank-soal-dan-pembahasan/` sebagai acuan utama.
4. **`pr-dan-kuis-pekan-9-15/`** (9 berkas: 7 PDF PR 2024, 1 PDF Kuis 4 2025, 1 ekspor solusi PR-07 2026)
   - Mencakup `PR-05` (*Buck Converter* + GaN 1 MHz), `PR-07` (*Boost Converter* + EIA E10 + ESR), `PR-08` (Blok Pembangun IC), `PR-09` (Penguat Diferensial + CMRR + *Cascode Tail*), `PR-10` (Penguat Diferensial PMOS beban aktif), `PR-11` (Op-Amp CMOS 2-tingkat), `PR-12` (Op-Amp *Folded-Cascode*), `Kuis-4 2025` (Penguat Diferensial beban aktif), dan ekspor solusi `PR-07 2026` (pasangan *source-coupled* beban aktif).
   - **Catatan Audit:** Beberapa solusi tulis tangan pada PR 8, PR 11, PR 12, serta tabel pada Kuis 4 memuat kekeliruan tanda tegangan, substitusi kuadrat, atau salah ketik tipe MOSFET yang seluruhnya diaudit dan dikoreksi di `../02-bank-soal-dan-pembahasan/Bank-Soal-03_Kurasi-PR-Pekan-9-15_dan_Kuis-4-EL3009.docx`.

## Catatan Buku Referensi

Buku acuan kuliah (*Microelectronic Circuits* Ed. 7 oleh Adel S. Sedra & Kenneth C. Smith serta *Power Electronics* oleh Daniel W. Hart) digunakan selama penyusunan untuk menjaga kesesuaian notasi, definisi parameter, dan nomor persamaan, tetapi berkas PDF buku berhak cipta tidak diunggah ke repositori publik ini.
