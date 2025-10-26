# IF5152 Computer Vision - Tugas Individu

Repositori ini berisi pengerjaan Tugas Individu IF5152 Computer Vision yang berisi materi berupa:
1.  Image Filtering
2.  Edge Detection
3.  Feature Points Detection
4.  Camera Geometry & Transformation

## Instalasi
Pastikan Anda memiliki Python dan `pip`. Download library yang dibutuhkan dengan perintah:

```bash
pip install opencv-python-headless scikit-image numpy matplotlib pandas
```

## Cara Menjalankan
Proyek ini terdiri dari 4 file .ipynb yang terpisah di dalam foldernya masing-masing.

1.  Buka terminal atau command prompt.
2.  Jalankan Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
3.  Buka dan jalankan sel-sel kode di dalam setiap file `.ipynb` berikut secara berurutan:
    * `01_filtering/01_filtering.ipynb`
    * `02_edge/02_edge.ipynb`
    * `03_featurepoints/03_featurepoints.ipynb`
    * `04_geometry/04_geometry.ipynb`

Setiap notebook akan memproses gambar dan menyimpan file output (gambar hasil dan file `.csv` berisi parameter/statistik) ke dalam folder `output` di dalam direktorinya masing-masing.

## Fitur Unik
Berikut adalah ringkasan fitur yang diimplementasikan di setiap notebook:

* **01_filtering:** Menerapkan 3 filter (Gaussian, Median, Sobel) dengan 3 variasi parameter. Menampilkan perbandingan hasil dalam grid 2x4 (Original + 3 variasi) untuk setiap jenis filter pada gambar `cameraman` dan `astronaut`.

* **02_edge:** Menerapkan 2 algoritma deteksi filter (Sobel dan Canny) dengan 3 variasi parameter (ukuran kernel untuk Sobel, threshold untuk Canny). Menampilkan perbandingan hasil dalam grid 2x4 pada gambar `coins` dan `chelsea`.

* **03_featurepoints:** Menerapkan 3 detektor (Harris, SIFT, FAST) pada gambar `checkerboard` dan `astronaut`. Menghitung dan menyimpan statistik lengkap (jumlah fitur, respons rata-rata, varians respons, dan sebaran X/Y) ke dalam file `.csv`.

* **04_geometry:** Mengimplementasikan homografi pada gambar `checkerboard`. Menghitung dan menyimpan matriks Homography (H) 3x3 ke dalam file `.txt` dan `.csv` sebagai output parameter.