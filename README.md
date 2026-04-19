# 🍬 Automated Candy Counting & Object Detection
An object detection system based on **Computer Vision** designed to automatically count candies within an image. This project utilizes the **YOLOv8** (You Only Look Once) architecture, trained on a custom dataset to facilitate automated inventory management.

*This project demonstrates the implementation of Deep Learning in the retail/manufacturing industry to accelerate stock-taking processes with high precision.*

## 📝 Project Description

The primary goal of this project is to build a model capable of identifying and counting various types of candies in a single scan. By leveraging the **YOLOv8** model, the system operates in **real-time** and provides accurate inventory reports. The project workflow includes dataset acquisition via **Roboflow**, model training in a GPU-accelerated environment (**Google Colab**), and visualization of detection results using **bounding boxes**.

## ✨ Key Features
  - **Real-time Object Detection**: Utilizing YOLOv8 for rapid and high-accuracy inference.
  - **Automated Inventory Reporting**: Integrated logic to sum the total number of detected items across all processed images.
  - **Roboflow Integration**: Seamless workflow for downloading and extracting annotated image datasets via API.
  - **High-Performance Training**: Optimized configuration for model training using NVIDIA Tesla T4 GPUs.
  - **Inference Visualization**: Visual outputs featuring class labels, bounding boxes, and confidence scores.

## 🛠️ Tech Stack & Implementation
  - **Computer Vision Framework**: Ultralytics YOLOv8
  - **Dataset Management**: Roboflow API
  - **Programming Language**: Python 3.x
  - **Image Processing**: OpenCV & PIL
  - **Environment**: Google Colab (GPU Accelerated)


## 📊 Methodology
  - **Data Acquisition**: Fetching annotated datasets from Roboflow using secure API keys.
  - **Model Training**: Training the YOLOv8 model for 50 epochs with a 640x640 input resolution.
  - **Validation**: Evaluating model performance based on the **mAP (mean Average Precision)** metric.
  - **Batch Inference**: Running detections on new image sets to validate the model's generalization capabilities.
  - **Inventory Summation**: Programming logic to extract detection counts and aggregate them into a final inventory report.

## ⚙️ Installation & Usage

### 1. Prerequisites (Roboflow API)

You must have a Roboflow API Key to download the dataset.

  - Obtain your key at: [Roboflow Dashboard](https://app.roboflow.com/).
  - Enter the key when prompted within the notebook.

### 2. Setup Environment

```bash
# Clone the repository
git clone https://github.com/Billy1205/candy-counting-object-detection.git
cd candy-counting-object-detection

# Install dependencies
pip install -r requirements.txt
```

### 3. Running the Analysis

1.  Open the notebook: `notebooks/Proyek_3_Candy_Counting.ipynb`.
2.  Ensure the **Runtime Type** is set to **GPU**.
3.  Execute the code cells to either train the model or perform inference using the pre-trained weights (`best.pt`).

***
# 🍬 Otomasi Perhitungan Permen & Deteksi Objek

Sistem deteksi objek berbasis **Computer Vision** untuk menghitung jumlah permen secara otomatis dalam sebuah gambar. Proyek ini menggunakan arsitektur **YOLOv8** (You Only Look Once) yang dilatih menggunakan dataset khusus untuk kebutuhan manajemen inventaris otomatis.

*Proyek ini mendemonstrasikan implementasi Deep Learning di bidang industri retail/manufaktur untuk mempercepat proses perhitungan stok (stock-taking) dengan akurasi tinggi.*

## 📝 Project Description

Tujuan utama proyek ini adalah membangun model yang mampu mengenali dan menghitung berbagai jenis permen dalam sekali pindai. Dengan memanfaatkan model **YOLOv8**, sistem ini dapat bekerja secara *real-time* dan memberikan laporan inventaris yang akurat. Alur kerja proyek meliputi akuisisi dataset dari **Roboflow**, pelatihan model di lingkungan GPU (**Google Colab**), hingga visualisasi hasil deteksi dengan *bounding boxes*.

## ✨ Key Features

  - **Real-time Object Detection**: Menggunakan YOLOv8 untuk deteksi yang cepat dan akurat.
  - **Automated Inventory Reporting**: Fungsi otomatis untuk menjumlahkan total item yang terdeteksi di seluruh gambar yang diproses.
  - **Roboflow Integration**: Alur kerja yang mulus untuk mengunduh dan mengekstrak dataset gambar yang sudah dianotasi.
  - **High-Performance Training**: Konfigurasi khusus untuk pelatihan model menggunakan GPU (Tesla T4).
  - **Inference Visualization**: Output gambar yang dilengkapi dengan label kelas dan skor kepercayaan (*confidence score*).

## 🛠️ Tech Stack & Implementation

  - **Computer Vision Framework**: Ultralytics YOLOv8.
  - **Dataset Management**: Roboflow API.
  - **Programming Language**: Python 3.x.
  - **Image Processing**: OpenCV & PIL.
  - **Environment**: Google Colab (with GPU acceleration).

## 📊 Methodology

  - **Data Acquisition**: Mengambil dataset teranotasi dari Roboflow menggunakan kunci API.
  - **Model Training**: Melatih model YOLOv8 selama 50 epoch dengan ukuran gambar 640x640 piksel.
  - **Validation**: Mengevaluasi performa model berdasarkan metrik mAP (mean Average Precision).
  - **Batch Inference**: Menjalankan deteksi pada sekumpulan gambar baru untuk memvalidasi kemampuan generalisasi model.
  - **Inventory Summation**: Logika pemrograman untuk mengekstrak angka dari hasil deteksi dan menggabungkannya menjadi laporan akhir.

## ⚙️ Installation & Usage

### 1. Prerequisites (Roboflow API)

Pastikan Anda memiliki API Key dari Roboflow untuk mengunduh dataset.

  - Dapatkan kunci di: [Roboflow Dashboard](https://app.roboflow.com/).
  - Masukkan kunci saat diminta dalam notebook.

### 2. Setup Environment

```bash
# Clone the repository
git clone https://github.com/Billy1205/candy-counting-object-detection.git
cd candy-counting-object-detection

# Install dependencies
pip install -r requirements.txt
```

### 3. Running the Analysis

1.  Buka notebook `notebooks/Proyek_3_Candy_Counting.ipynb`.
2.  Pastikan *Runtime* diatur ke **GPU**.
3.  Jalankan sel kode untuk melatih model atau langsung lakukan inferensi menggunakan bobot (*weights*) `best.pt`.
