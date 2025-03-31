# Tugas Kelompok Linear dan Polynomial Regression

# Startup-50
## Anggota Tim (Kelompok 4)
- Glenn Hakim (2208107010072)
- Ahmad Syah Ramadhan (2208107010033)
- Andika Pebriansyah (2208107010058)
- Nisa Rianti (2208107010018)
- Nuri Masyithah (2208107010006)

# Gambaran Proyek
Dalam era digital yang semakin berkembang, startup memainkan peran penting dalam mendorong inovasi dan pertumbuhan ekonomi. Namun, kesuksesan sebuah startup tidak hanya ditentukan oleh ide yang inovatif, tetapi juga oleh faktor-faktor finansial dan strategis yang mendukung operasionalnya.
Dalam dunia bisnis, pemahaman tentang faktor-faktor yang mempengaruhi kesuksesan startup sangat penting. Dengan analisis data, kita dapat mengidentifikasi pola dan tren yang berkontribusi terhadap keberhasilan perusahaan rintisan. Dataset yang digunakan dalam analisis ini berasal dari Kaggle dan mencakup informasi tentang 50 startup, termasuk pengeluaran R&D, pemasaran, dan keuntungan yang diperoleh.

# Tujuan
1. Tujuan dari analissi ini adalah untuk:
2. Memahami faktor-faktor utama yang berkontribusi terhadap keberhasilan startup.
3. Menggunakan teknik analisis data untuk mengidentifikasi hubungan antara variabel dalam dataset.
4. Menerapkan model Machine Learning untuk memprediksi keuntungan startup berdasarkan variabel yang tersedia.

# Deskripsi Dataset
Dataset yang digunakan dalam analisis ini adalah 50_Startups.csv, yang berisi informasi tentang investasi perusahaan rintisan dan keuntungan yang diperoleh. Variabel yang tersedia dalam dataset ini antara lain:
- R&D Spend: Investasi dalam penelitian dan pengembangan.
- Administration: Biaya administrasi perusahaan.
- Marketing Spend: Biaya pemasaran.
- State: Lokasi perusahaan (New York, California, Florida).
- Profit: Keuntungan yang diperoleh.

# Proses Persiapan Data
1. Data Loading
   - Menggunakan pandas untuk membaca dataset 50_Startups.csv
2. Data Understanding
   - Menampilkan sampel data dengan .head()
   - Memeriksa tipe data dan informasi dataset dengan .info()
   - Menampilkan statistik deskriptif dengan .describe()
   - Mengecek nilai yang hilang dengan .isnull().sum()
3. Data Cleaning & Preprocessing
   - Handling Missing Values: Memeriksa apakah ada nilai yang hilang dan melakukan penanganan jika diperlukan
   - Categorical Feature Encoding:Menggunakan OneHotEncoder untuk mengubah data kategorikal menjadi numerik
   - Feature Scaling:Menggunakan StandardScaler untuk menormalkan data numerik
   - Feature Engineering: Menggunakan PolynomialFeatures untuk menciptakan fitur tambahan jika diperlukan.
4. Data Splitting
   - Dataset dibagi menjadi training set dan test set menggunakan train_test_split() dari sklearn.model_selection

# Teknologi yang Digunakan
-  Bahasa Pemrograman: Python
-  Library & Framework:
  - pandas → Loading dan manipulasi dataset
  - numpy → Operasi numerik
  - matplotlib & seaborn → Visualisasi data
  - sklearn.model_selection → train_test_split, GridSearchCV
  - sklearn.preprocessing → StandardScaler, OneHotEncoder, PolynomialFeatures
  - sklearn.pipeline → Pipeline untuk preprocessing otomatis
  - sklearn.linear_model → Model regresi linear
  - sklearn.metrics → Evaluasi model (MSE, R2 score, dll.)
