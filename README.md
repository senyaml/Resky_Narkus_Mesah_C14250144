# 🚗 **Proyek Analisis Data Toyota Corolla -- KNIME Workflow**

**Oleh: C14250144**\
**Dataset:** *ToyotaCorolla.csv*\
**Workflow:** *Projek_DAE_UAS_C14250144_Toyota.knwf*

------------------------------------------------------------------------

## 📌 **Overview Proyek**

Proyek ini melakukan *Data Preparation*, *Preprocessing*, *Feature
Engineering*, *Agregasi*, serta *Visualisasi* menggunakan **KNIME**.\
Fokus utama proyek ini adalah menganalisis hubungan **KM, Harga,
Tahun**, serta membuat kategori berdasarkan **KM** melalui *Rule
Engine*.

------------------------------------------------------------------------

# 🧱 **1. Data Preparation**

### 🔶 *Node yang digunakan*

  *CSV Reader*      Membaca dataset ToyotaCorolla.csv
  *Column Filter*   Memilih kolom *Price*, *Mfg_Year*, dan *KM*
  *Column Renamer*  Menstandarkan / merapikan nama kolom

### 🔧 *Hasil Tahap Preparation*

✔ Dataset bersih\
✔ Kolom telah difilter sesuai kebutuhan\
✔ Nama kolom sudah rapi dan seragam

------------------------------------------------------------------------

# 🛠 **2. Preprocessing**

Pada tahap ini dilakukan filtering berdasarkan tahun tertentu serta
pembuatan fitur kategori menggunakan **Rule Engine**.

### 🔶 *Row Filter*

-   **Tahun 2004**
-   **Tahun 2002**

### 🔶 *Rule Engine (kategori KM)*

Aturan kategori KM:

    $KM$ <= 20000 => "rendah"
    $KM$ <= 99000 => "tinggi"
    TRUE => "medium"

📝 *Node ini menghasilkan kolom baru bernama* **kategori_km**

------------------------------------------------------------------------

# 📊 **3. Agregasi (GroupBy)**

### 🔶 *GroupBy 1 -- Rata-rata Harga Tahun 2004*

Menghasilkan: - Average Price - Distribusi untuk visualisasi Pie Chart &
Line Plot

### 🔶 *GroupBy 2 -- Rata-rata Harga per Tahun*

Untuk visualisasi tren harga:

-   Line Plot (Harga vs Tahun)
-   Bar Chart (Rata-rata Harga)

### 🔶 *GroupBy 3 -- Rata-rata Harga berdasarkan kategori KM*

Digunakan untuk: - Bar Chart (Average KM Category) - Line Plot - Pie
Chart (Distribusi harga kategori)

------------------------------------------------------------------------

# 📈 **4. Visualisasi**

Visualisasi dilakukan untuk memahami pola & tren data.

### 🎯 *Node Visualisasi*

  Visual          Fungsi
  --------------- ----------------------------------------------
  **Line Plot**   Tren rata-rata harga & KM
  **Bar Chart**   Membandingkan nilai rata-rata antar kategori
  **Pie Chart**   Proporsi kategori tahun atau kategori KM

### ✨ *Insight Visualisasi*

-   Tahun produksi lebih muda → harga lebih tinggi\
-   KM rendah → harga lebih mahal\
-   Kategori KM *rendah / medium / tinggi* menunjukkan pola distribusi
    yang jelas

------------------------------------------------------------------------

# 🧩 **5. Insight & Interpretasi**

### 🔍 *Temuan*

-   KM memiliki pengaruh kuat terhadap harga jual.
-   Tahun produksi berbanding lurus dengan harga.
-   Perbedaan kategori KM terlihat jelas pada visualisasi (harga menurun
    seiring meningkatnya KM).

### 💡 *Interpretasi*

Workflow sukses mengubah data mentah menjadi insight visual yang mudah
dipahami.\
Kategori KM dari *Rule Engine* sangat membantu segmentasi kendaraan
berdasarkan tingkat pemakaian.

------------------------------------------------------------------------

# 🏁 **6. Kesimpulan**

-   Proyek KNIME berhasil melakukan *Preparation → Preprocessing →
    Agregasi → Visualisasi* secara lengkap.
-   Aturan kategori KM sudah benar dan mencerminkan kondisi sebenarnya.
-   Workflow dapat dikembangkan menjadi model prediksi harga atau
    klasifikasi tingkat KM di masa depan.

------------------------------------------------------------------------

# 📦 **Download Workflow**
*https://github.com/senyaml/Resky_Narkus_Mesah_C14250144/releases/download/download/Projek_DAE_UAS_C14250144_Toyota.zip*
