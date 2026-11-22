# **SOLUSI PEKERJAAN RUMAH 07 — EL3009 ELEKTRONIKA 2**

**Topik:** Analisis Bias DC, Rangkaian Ekivalen Sinyal Kecil, dan Batas Operasi Linier Penguat MOSFET Beban Aktif  
**Penyusun:** Arsip Mahasiswa EL3009 (Anonim)
Semester I 2026/2027
Tenggat Pengumpulan: Selasa, 10 November 2026

# **1\. Spesifikasi Parameter dan Identifikasi Topologi Rangkaian**

Rangkaian pada soal merupakan penguat berbasis pasangan sumber-bersama (source-coupled pair) M₁ dan M₂ yang menggunakan beban aktif PMOS M₃. Rangkaian dicatu oleh sumber tegangan DC simetris V\_DD \= \+3 V dan V\_SS \= −3 V, serta sumber arus ekor (tail current source) I\_SS \= 200 μA.

## **Tabel 1\. Parameter Fisik dan Konfigurasi Terminal Transistor**

| Perangkat | Tipe | Parameter Fisik | Konfigurasi Terminal pada Rangkaian |
| :---- | :---- | :---- | :---- |
| **M₁** | NMOS (Identik dengan M₂) | k₁ \= 200 μA/V², V\_t1 \= 1.0 V, λ₁ \= 1/(50 V) \= 0.02 V⁻¹ (V\_A1 \= 50 V) | Gate (G₁) ke sumber masukan v\_i (bias DC V\_G1 \= 0 V); Drain (D₁) ke node keluaran v\_o; Source (S₁) ke node bersama S |
| **M₂** | NMOS (Identik dengan M₁) | k₂ \= 200 μA/V², V\_t2 \= 1.0 V, λ₂ \= 1/(50 V) \= 0.02 V⁻¹ (V\_A2 \= 50 V) | Gate (G₂) ke ground (0 V); Drain (D₂) ke ground (0 V); Source (S₂) ke node bersama S |
| **M₃** | PMOS (Beban Aktif) | k' \= 30 μA/V², V\_t3 \= −1.0 V (\|V\_t3\| \= 1.0 V), λ₃ \= 1/(30 V) V⁻¹ (V\_A3 \= 30 V) | Source (S₃) ke V\_DD (+3 V); Gate (G₃) ke ground (0 V); Drain (D₃) ke node keluaran v\_o |

# **2\. Jawaban Bagian (a): Penentuan Rasio W₃/L₃ untuk Bias V\_o \= 0 V**

**Tujuan:** Menentukan rasio dimensi kanal W₃/L₃ pada transistor PMOS M₃ sedemikian sehingga tegangan DC pada node keluaran dibias tepat pada V\_o \= 0 V saat sinyal masukan bernilai nol (v\_i \= 0 V).

## **Prosedur Analisis Bias DC (Tahap demi Tahap)**

1. **Pembagian Arus Bias pada Pasangan Simetris M₁ dan M₂:**  
   Pada kondisi bias DC (v\_i \= 0 V) dan tegangan keluaran V\_o \= 0 V:  
   * Tegangan gate kedua transistor bernilai identik: V\_G1 \= V\_G2 \= 0 V.  
   * Tegangan drain kedua transistor bernilai identik: V\_D1 \= V\_o \= 0 V dan V\_D2 \= 0 V.  
   * Terminal source kedua transistor terhubung pada satu node yang sama: V\_S1 \= V\_S2 \= V\_S.

   

   Karena M₁ dan M₂ merupakan pasangan transistor yang identik (matche

d devices) serta memiliki tegangan V\_GS1 \= V\_GS2 dan V\_DS1 \= V\_DS2 yang persis sama, maka arus sumber ekor I\_SS \= 200 μA terbagi dua sama besar secara eksak (bahkan ketika efek modulasi panjang kanal λ\_n diperhitungkan):

* **I\_D1 \= I\_D2 \= I\_SS / 2 \= 200 μA / 2 \= 100 μA**

Berdasarkan Hukum Arus Kirchhoff (KCL) pada node keluaran V\_o (tanpa beban eksternal), seluruh arus drain dari M₃ mengalir masuk ke drain M₁:

* **I\_D3 \= I\_D1 \= 100 μA**  
2. **Verifikasi Titik Kerja DC pada M₁ dan M₂ (Memastikan Operasi Saturasi):**  
   Dengan menggunakan persamaan arus drain MOSFET di daerah saturasi, I\_D1 \= (1/2) · k · (V\_GS1 − V\_t1)² \= (1/2) · k · V\_OV1², tegangan overdrive V\_OV1 dan V\_OV2 diperoleh sebesar:  
   * **V\_OV1 \= V\_OV2 \= √(2 · I\_D1 / k) \= √(2 × 100 μA / 200 μA/V²) \= √(1.0 V²) \= 1.0 V**  
   * **V\_GS1 \= V\_GS2 \= V\_t1 \+ V\_OV1 \= 1.0 V \+ 1.0 V \= 2.0 V**  
   * **V\_S \= V\_G1 − V\_GS1 \= 0 V − 2.0 V \= −2.0 V**

   

   Pemeriksaan syarat saturasi M₁ dan M₂

:

* **V\_DS1 \= V\_DS2 \= 0 V − (−2.0 V) \= 2.0 V ≥ V\_OV1 (1.0 V)** ⇒ Terbukti M₁ dan M₂ beroperasi di **daerah saturasi**.  
3. **Pemeriksaan Daerah Operasi dan Tegangan Kerja Transistor PMOS M₃:**  
   Untuk transistor M₃, tegangan pada setiap terminalnya adalah V\_S3 \= \+3.0 V, V\_G3 \= 0 V, dan V\_D3 \= V\_o \= 0 V:  
   * **V\_SG3 \= V\_S3 − V\_G3 \= 3.0 V − 0 V \= 3.0 V**  
   * **V\_OV3 \= V\_SG3 − \|V\_t3\| \= 3.0 V − 1.0 V \= 2.0 V**  
   * **V\_SD3 \= V\_S3 − V\_D3 \= 3.0 V − 0 V \= 3.0 V**

   

   Pemeriksaan syara

t saturasi M₃:

* **V\_SD3 \= 3.0 V ≥ V\_OV3 (2.0 V)** ⇒ Terbukti M₃ beroperasi di **daerah saturasi**.  
4. **Perhitungan Rasio W₃/L₃:**  
   * **Metode 1 (Persamaan Bias DC Standar — Mengabaikan λ₃ pada Perhitungan Bias DC):**  
     I\_D3 \= (1/2) · k' · (W₃/L₃) · (V\_SG3 − \|V\_t3\|)²  
     100 μA \= (1/2) × (30 μA/V²) × (W₃/L₃) × (2.0 V)²  
     100 μA \= 60 μA × (W₃/L₃)  
     **W₃/L₃ \= 100 / 60 \= 5/3 ≈ 1.67**  
   * **Metode 2 (Persamaan Bias DC Eksak — Menyertakan Faktor Modulasi Panjang Kanal 1 \+ λ₃·V\_SD3):**  
     Apabila efek modulasi panjang kanal (λ₃ \= 1/30 V⁻¹) disertakan agar arus DC I\_D3 \= 100 μA pada V\_o \= 0 V terpenuhi secara presisi:  
     I\_D3 \= (1/2) · k' · (W₃/L₃) · (V\_SG3 − \|V\_t3\|)² · (1 \+ λ₃ · V\_SD3)  
     Faktor modulasi panjang kanal: (1 \+ λ₃ · V\_SD3) \= 1 \+ (3.0 V / 30 V) \= 1.1  
     100 μA \= 60 μA × 1.1 × (W₃/L₃) \= 66 μA × (W₃/L₃)  
     **W₃/L₃ \= 100 / 66 \= 50/33 ≈ 1.52**

# **3\. Jawaban Bagian (b): Penyederhanaan Rangkaian Ekivalen, R\_o, dan v\_o/v\_i**

## **3.1 Perhitungan Parameter Sinyal Kecil Masing-Masing Transistor**

Pada arus titik kerja I\_D1 \= I\_D2 \= I\_D3 \= 100 μA \= 0.1 mA, parameter sinyal kecil untuk masing-masing transistor adalah:

1. **Transkonduktansi (g\_m1 dan g\_m2):**  
   * **g\_m1 \= g\_m2 \= g\_m \= √(2 · k · I\_D1) \= √(2 × 200 μA/V² × 100 μA) \= 200 μA/V \= 0.2 mA/V**  
   * **1 / g\_m2 \= 1 / (0.2 mA/V) \= 5.0 kΩ**  
2. **Resistansi Keluaran Sinyal Kecil (r\_o1, r\_o2, dan r\_o3):**  
   * **r\_o1 \= r\_o2 \= r\_o \= V\_A1 / I\_D1 \= 50 V / 100 μA \= 500 kΩ**  
   * **r\_o3 \= V\_A3 / I\_D3 \= 30 V / 100 μA \= 300 kΩ**

## **3.2 Penyederhanaan Bertahap Menggunakan Rangkaian Ekivalen Sinyal Kecil**

Untuk memudahkan analisis tanpa harus menyelesaikan persamaan seluruh transistor secara simultan, rangkaian tiga transistor direduksi melalui empat tahap rangkaian ekivalen berikut:

## **Tabel 2\. Tahapan Reduksi Menuju Rangkaian Ekivalen Sinyal Kecil**

| Tahap Reduksi | Bagian yang Disederhanakan | Dasar Fisik / Sinyal Kecil | Bentuk Ekivalen Hasil Reduksi |
| :---- | :---- | :---- | :---- |
| **Tahap 1** | Catu DC (+3 V, −3 V) dan Sumber Arus Ekor 200 μA | Tegangan DC konstan memiliki perubahan AC ΔV \= 0; sumber arus DC ideal memiliki ΔI \= 0 | Node \+3 V dan −3 V menjadi **ground AC (0 V)**; sumber arus 200 μA menjadi **rangkaian terbuka (open circuit)** |
| **Tahap 2** | Transistor Beban Aktif PMOS M₃ | Source S₃ di ground AC (+3 V) dan Gate G₃ di ground (0 V), sehingga v\_sg3 \= 0 V dan sumber arus g\_m3·v\_sg3 \= 0 A (terbuka) | M₃ digantikan oleh satu **resistor beban pasif r\_o3 \= 300 kΩ** yang terhubung antara node keluaran v\_o dan ground AC |
| **Tahap 3** | Transistor NMOS M₂ | Gate G₂ dan Drain D₂ keduanya di ground (v\_g2 \= v\_d2 \= 0 V). Dilihat dari terminal Source S₂, arus yang mengalir ke ground adalah i\_s2 \= g\_m2·v\_s \+ v\_s/r\_o2 | M₂ digantikan oleh satu **resistor degenerasi source R\_S \= (1/g\_m2) ∥ r\_o2 \= 5 kΩ ∥ 500 kΩ ≈ 4.95 kΩ** (atau pendekatan R\_S ≈ 1/g\_m2 \= 5.0 kΩ) dari Source M₁ ke ground |
| **Tahap 4** | Rangkaian Keseluruhan (M₁ \+ R\_S \+ r\_o3) | Penguat Common-Source M₁ dengan degenerasi source R\_S dan beban drain r\_o3 diubah menjadi **Rangkaian Ekivalen Norton** pada node v\_o | Sumber arus terkendali **G\_m·v\_i** (dari node v\_o ke ground) yang diparalelkan dengan resistansi drain **R\_d1** dan beban **r\_o3** (**R\_o \= R\_d1 ∥ r\_o3**) |

## **3.3 Perhitungan Resistansi Keluaran (R\_o)**

Untuk menghitung resistansi keluaran R\_o, sumber tegangan masukan dinolkan (v\_i \= 0 V, sehingga Gate M₁ terhubung ke ground AC). Berdasarkan hasil penyederhanaan pada Tabel 2, resistansi keluaran R\_o merupakan hubungan paralel antara resistansi yang terlihat ke dalam drain M₁ (R\_d1) dan resistansi drain M₃ (r\_o3):

* **R\_o \= R\_d1 ∥ r\_o3**

Untuk penguat Common-Source (M₁) dengan resistansi degenerasi source sebesar R\_S, resistansi yang terlihat ke arah drain M₁ (R\_d1) dinyatakan oleh rumus standar:

* R\_d1 \= r\_o1 \+ R\_S · (1 \+ g\_m1 · r\_o1)

Karena M₁ dan M₂ identik (g\_m1 \= g\_m2 \= g\_m dan r\_o1 \= r\_o2 \= r\_o), substitusi bentuk eksak **R\_S \= (1/g\_m) ∥ r\_o \= r\_o / (1 \+ g\_m · r\_o)** ke dalam persamaan R\_d1 menghasilkan penyederhanaan aljabar yang eksak:

* **R\_d1 \= r\_o \+ \[r\_o / (1 \+ g\_m · r\_o)\] · (1 \+ g\_m · r\_o) \= r\_o \+ r\_o \= 2 · r\_o1**

*(Catatan: Pendekatan standar buku teks dengan R\_S ≈ 1/g\_m2 dan R\_d1 ≈ r\_o1 · (1 \+ g\_m1 · R\_S) \= r\_o1 · (1 \+ g\_m1/g\_m2) \= 2 · r\_o1 memberikan hasil yang sama persis.)*

Substitusi nilai numerik r\_o1 \= 500 kΩ dan r\_o3 \= 300 kΩ:

* **R\_d1 \= 2 × 500 kΩ \= 1000 kΩ \= 1.0 MΩ**  
* **R\_o \= R\_d1 ∥ r\_o3 \= 1000 kΩ ∥ 300 kΩ \= (1000 × 300\) / (1000 \+ 300\) kΩ \= 3000/13 kΩ ≈ 230.77 kΩ**

## **3.4 Perhitungan Penguatan Tegangan Sinyal Kecil (v\_o / v\_i)**

Dengan menggunakan **Rangkaian Ekivalen Norton** pada node keluaran v\_o (Tahap 4 pada Tabel 2), transkonduktansi hubung-singkat G\_m dicari terlebih dahulu dengan menghubungsingkatkan node keluaran ke ground AC (v\_o \= 0 V) dan menghitung rasio arus hubung-singkat i\_o yang mengalir masuk ke drain M₁ terhadap v\_i.

1. **Persamaan KCL pada Node Source Bersama (v\_s) saat v\_o \= 0 V:**  
   Arus yang meninggalkan drain/source M₁ menuju node v\_s sama dengan arus yang mengalir melalui R\_S ke ground:  
   * g\_m1 · (v\_i − v\_s) \+ (0 − v\_s) / r\_o1 \= v\_s / R\_S  
   * g\_m1 · v\_i \= v\_s · \[g\_m1 \+ (1 / r\_o1) \+ (1 / R\_S)\]  
2. **Substitusi Konduktansi Ekivalen 1/R\_S:**  
   Karena 1 / R\_S \= g\_m2 \+ (1 / r\_o2) \= g\_m1 \+ (1 / r\_o1) (akibat kesimetrian M₁ dan M₂), maka:  
   * g\_m1 · v\_i \= 2 · v\_s · \[g\_m1 \+ (1 / r\_o1)\]  
   * **v\_s · \[g\_m1 \+ (1 / r\_o1)\] \= (1/2) · g\_m1 · v\_i**  
3. **Arus Hubung-Singkat Drain M₁ (i\_o) dan Transkonduktansi Efektif (G\_m):**  
   * i\_o \= g\_m1 · (v\_i − v\_s) − (v\_s / r\_o1) \= g\_m1 · v\_i − v\_s · \[g\_m1 \+ (1 / r\_o1)\]  
   * i\_o \= g\_m1 · v\_i − (1/2) · g\_m1 · v\_i \= (1/2) · g\_m1 · v\_i  
   * **G\_m \= i\_o / v\_i \= (1/2) · g\_m1 \= (1/2) × (0.2 mA/V) \= 0.1 mA/V \= 100 μA/V**  
     *(Catatan: Rumus pendekatan degenerasi source G\_m ≈ g\_m1 / (1 \+ g\_m1 · R\_S) \= g\_m1 / (1 \+ g\_m1/g\_m2) \= (1/2) · g\_m1 \= 0.1 mA/V juga menghasilkan nilai yang identik.)*  
4. **Perhitungan Penguatan Tegangan (v\_o / v\_i):**  
   Berdasarkan rangkaian ekivalen Norton, tegangan keluaran adalah v\_o \= −i\_o · R\_o \= −G\_m · R\_o · v\_i, sehingga:  
   * **v\_o / v\_i \= −G\_m · R\_o \= −(0.1 mA/V) × (3000/13 kΩ) \= −300/13 V/V ≈ −23.08 V/V**  
     *(Catatan Tambahan: Apabila efek r\_o1 diabaikan terhadap pembagian arus sinyal keluaran sehingga beban hanya r\_o3, maka pendekatan kasar memberikan v\_o / v\_i ≈ −G\_m · r\_o3 \= −(0.1 mA/V) × (300 kΩ) \= −30.0 V/V.)*

# **4\. Jawaban Bagian (c): Perkiraan v\_o(min) dan v\_o(max) (Daerah Operasi Linier)**

**Konsep Dasar:** Daerah operasi linier (linear region of operation) dari sebuah rangkaian penguat adalah rentang tegangan keluaran \[v\_o(min), v\_o(max)\] di mana seluruh transistor pada jalur penguatan (M₁, M₂, dan M₃) tetap beroperasi di **daerah saturasi (aktif)**. Apabila v\_o melampaui batas tersebut, salah satu transistor akan memasuki daerah triode sehingga penguatan tegangan turun secara drastis.

## **Prosedur Penentuan Batas Operasi Linier**

1. **Batas Atas Tegangan Keluaran v\_o(max) — Dibatasi oleh Saturasi PMOS M₃:**  
   Ketika tegangan keluaran v\_o bergerak naik mendekati \+3.0 V, tegangan source-ke-drain pada M₃ (v\_SD3 \= V\_S3 − v\_o) mengecil. Agar M₃ tetap berada di daerah saturasi, harus dipenuhi syarat:  
   * v\_SD3 ≥ V\_SG3 − \|V\_t3\| \= V\_OV3 ⇔ V\_S3 − v\_o ≥ V\_OV3  
   * Secara ekuivalen, tegangan drain M₃ (v\_D3 \= v\_o) tidak boleh melebihi V\_G3 \+ \|V\_t3\|:  
   * v\_o ≤ V\_G3 \+ \|V\_t3\| \= 0 V \+ 1.0 V \= \+1.0 V  
   * **v\_o(max) \= \+1.0 V**  
     *(Di atas \+1.0 V, transistor beban M₃ keluar dari daerah saturasi dan masuk ke daerah triode.)*  
2. **Batas Bawah Tegangan Keluaran v\_o(min) — Dibatasi oleh Saturasi NMOS M₁:**  
   Ketika tegangan keluaran v\_o bergerak turun (menjadi negatif), tegangan drain-ke-source pada M₁ (v\_DS1 \= v\_o − v\_S) mengecil. Agar transistor M₁ tetap berada di daerah saturasi, harus dipenuhi syarat:  
   * v\_DS1 ≥ v\_GS1 − V\_t1 ⇔ v\_D1 − v\_S ≥ v\_G1 − v\_S − V\_t1 ⇔ **v\_o ≥ v\_G1 − V\_t1**

   

   Terdapat dua metode perkiraan untuk menentuka

n v\_o(min):

* **Perkiraan Orde Pertama (Pendekatan Titik Bias DC, v\_G1 \= v\_i ≈ 0 V):**  
  Karena penguatan tegangan cukup besar (\|A\_v\| \= 23.08 V/V), perubahan tegangan masukan v\_i sangat kecil dibandingkan tegangan ambang V\_t1 \= 1.0 V. Dengan menggunakan nilai bias DC (V\_G1 \= 0 V, atau V\_S \+ V\_OV1 \= −2.0 V \+ 1.0 V):  
  **v\_o(min) ≈ V\_G1 − V\_t1 \= 0 V − 1.0 V \= −1.0 V**  
* **Perkiraan Orde Kedua (Menyertakan Simpangan Masukan v\_G1 \= v\_i \= v\_o / A\_v):**  
  Apabila kenaikan kecil pada tegangan gate M₁ sebesar v\_G1 \= v\_i \= v\_o / A\_v diperhitungkan ketika M₁ mencapai tepi saturasi:  
  v\_o(min) \= \[v\_o(min) / A\_v\] − V\_t1  
  **v\_o(min) \= −V\_t1 / \[1 − (1 / A\_v)\] \= −1.0 V / \[1 − (1 / −23.08)\] \= −1.0 V / 1.0433 ≈ −0.96 V**

# **5\. Tabel Ringkasan Akhir Seluruh Jawaban**

| Bagian | Parameter yang Ditanyakan | Rumus Utama | Hasil Perhitungan Akhir |
| :---- | :---- | :---- | :---- |
| **(a)** | Rasio dimensi **W₃/L₃** untuk bias V\_o \= 0 V | I\_D3 \= (1/2)·k'·(W₃/L₃)·V\_OV3²·(1 \+ λ₃·V\_SD3) | **5/3 ≈ 1.67** (DC standar) atau **50/33 ≈ 1.52** (dengan λ₃) |
| **(b)** | Resistansi keluaran penguat (**R\_o**) | R\_o \= R\_d1 ∥ r\_o3 \= (2·r\_o1) ∥ r\_o3 | **3000/13 kΩ ≈ 230.77 kΩ** |
| **(b)** | Penguatan tegangan sinyal kecil (**v\_o / v\_i**) | v\_o / v\_i \= −G\_m · R\_o \= −(1/2 · g\_m1) · R\_o | **−300/13 V/V ≈ −23.08 V/V** (atau −30.0 V/V jika r\_o1 → ∞) |
| **(c)** | Batas bawah daerah operasi linier (**v\_o(min)**) | v\_o ≥ v\_G1 − V\_t1 | **−1.0 V** (pendekatan DC) atau **−0.96 V** (koreksi v\_i) |
| **(c)** | Batas atas daerah operasi linier (**v\_o(max)**) | v\_o ≤ V\_G3 \+ \|V\_t3\| | **\+1.0 V** |

