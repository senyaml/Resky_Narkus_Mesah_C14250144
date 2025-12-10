# Proyek Analisis Data Toyota Corolla (DAE)

## 📌 Informasi Proyek
**Nama Proyek:** Analisis Data Eksploratif Toyota Corolla  
**Disusun oleh:** *C14250144*  
**Dataset:** `ToyotaCorolla.csv`  
**Platform:** KNIME

---

## 📊 Tujuan Proyek
Proyek ini bertujuan melakukan:
- Exploratory Data Analysis (EDA)
- Preprocessing data
- Feature engineering dan agregasi
- Visualisasi data  
pada dataset **Toyota Corolla**, untuk menemukan pola harga, faktor yang mempengaruhi harga, serta tren penting lainnya.

---

## ⚙️ Alur Kerja (Workflow) – *KNIME*
Workflow terbagi menjadi **tiga tahap besar**:

---

## 1️⃣ Preparation Data
| Node | Fungsi |
|------|--------|
| **CSV Reader** | Memuat data mentah dari dataset. |
| **Column Filter** | Memilih kolom penting untuk analisis. |
| **Row Filter** | Menyaring data sesuai kriteria tertentu. |
| **String to Number / Number to String** | Menjamin tipe data sesuai kebutuhan analisis. |

---

## 2️⃣ Preprocessing Data
| Node | Fungsi |
|------|--------|
| **GroupBy (banyak node)** | Menghitung rata-rata, jumlah, atau agregasi lainnya berdasarkan kategori (contoh: Fuel_Type, Age). |
| **Rule Engine** | Membuat kategori baru (contoh: kategori Harga, kategori KM). |
| **Column Renamer** | Memberi nama baru pada kolom hasil agregasi untuk memudahkan analisis. |

---

## 3️⃣ Visualisasi Data (EDA)
| Visualisasi | Fungsi |
|------------|--------|
| **Line Plot** | Menampilkan tren harga rata-rata berdasarkan tahun produksi. |
| **Bar Chart** | Membandingkan harga rata-rata antar kategori (Fuel Type, Doors, dan lainnya). |
| **Pie Chart** | Menunjukkan proporsi kategori baru dari Rule Engine (contoh: kategori harga). |

---

## 🔍 Hasil Analisis & Insight

### ⭐ Insight Utama
- **Harga mobil menurun seiring bertambahnya usia mobil.**
- Distribusi harga menunjukkan mayoritas mobil berada pada kategori **Sedang** dan **Murah**.

### 🧠 Interpretasi
- Proses EDA berhasil mengubah data mentah menjadi insight yang jelas.
- Rule Engine membantu menyederhanakan variabel harga menjadi kategori yang mudah dipahami.
- Tahun produksi adalah prediktor harga paling kuat, namun variabel KM dan spesifikasi juga berpengaruh.

---

## ✔️ Kesimpulan
Analisis menunjukkan bahwa:
- Harga Toyota Corolla sangat dipengaruhi oleh **Tahun Produksi**, **KM**, dan beberapa variabel kategoris.
- Workflow KNIME yang dibuat sudah lengkap dan mampu menghasilkan insight yang akurat.
- Dataset cocok dijadikan dasar untuk modeling lanjutan seperti **regresi harga** atau **klasifikasi kategori harga**.

---

## 📁 Struktur Repository
```
├── README.md
├── ToyotaCorolla.csv
└── Projek_UAS_Toyota.knwf
```

---

## 🏁 Catatan Akhir
Jika ingin menambahkan:
- gambar workflow,
- badge GitHub,
- tema warna markdown,
- atau versi PDF,

tinggal bilang saja!
