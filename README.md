# 📊 Ringkasan Materi Pra-UTS: Data Processing & Machine Learning Dasar

## 📁 1. Data Processing dengan `pandas`

### ✅ Tujuan:
Melakukan manipulasi data secara efisien untuk persiapan analisis dan machine learning.

### 📌 Materi Inti:
- **Import Dataset**: `pd.read_csv()`, `pd.read_excel()`
- **Eksplorasi Data**: `df.head()`, `df.info()`, `df.describe()`, `df.shape`
- **Seleksi Kolom/Baris**: 
  - Kolom: `df['kolom']` atau `df[['kolom1', 'kolom2']]`
  - Baris: `df.loc[]`, `df.iloc[]`
- **Missing Value Handling**: 
  - Deteksi: `df.isnull().sum()`
  - Mengisi nilai: `df.fillna()`
  - Menghapus baris: `df.dropna()`
- **Encoding Kategori**:
  - Manual: `df['kolom'].map()`
  - Otomatis: `pd.get_dummies()`, `LabelEncoder()`

---

## 📈 2. Visualisasi Data dengan `matplotlib`

### ✅ Tujuan:
Memahami distribusi data dan hubungan antar fitur.

### 📌 Materi Inti:
- **Import**: `import matplotlib.pyplot as plt`
- **Plot Dasar**: `plt.plot()`, `plt.bar()`, `plt.hist()`, `plt.scatter()`
- **Customisasi**:
  - Label sumbu: `plt.xlabel()`, `plt.ylabel()`
  - Judul: `plt.title()`
  - Legend: `plt.legend()`
- **Tampilkan Plot**: `plt.show()`

---

## 🧠 3. Naive Bayes Classifier

### ✅ Tujuan:
Klasifikasi berbasis probabilitas menggunakan Teorema Bayes.

### 📌 Karakteristik:
- Cocok untuk data teks dan klasifikasi cepat.
- Asumsi: Fitur saling independen.

### 📌 Implementasi:
```python
from sklearn.naive_bayes import GaussianNB
model = GaussianNB()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
