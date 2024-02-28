
# The Art of Prompt Engineering
## Author : Cognitive class AI (Svitlana Kramar)
#### Mentee assignment from IBM Advance AI @ Infinite Learning Course completion of "Natural Language Processing with Hugging Face Transformers" from CognitiveClass.ai
### Mentee info
#### Name : Marco Philips Sirait
#### Program : IBM Advance AI (MSIB Batch 6) with Infinite Learning

---

Bahasa Inggris / ENG / English:
---
This Guided Project will walk you through some of the applications of Hugging Face Transformers in Natural Language Processing (NLP).

Hugging Face Transformers package is very popular and versatile Python library that provides pre-trained models for a variety of applications in NLP, as well other areas such as image analysis, audio analysis, multimodal analysis (optical character recognition, video classification, visual question answering and many more).

---

Bahas Indonesia / IDN:
---
Projek Panduan ini akan memandu Anda melalui beberapa aplikasi Hugging Face Transformers dalam Pemrosesan Bahasa Alami (NLP).

Paket Hugging Face Transformers adalah pustaka Python yang sangat populer dan serbaguna yang menyediakan model-model yang telah di-pre-train untuk berbagai aplikasi dalam NLP, serta area lain seperti analisis gambar, analisis audio, analisis multimodal (pengenalan karakter optik, klasifikasi video, pertanyaan visual dan banyak lagi).

---
---
---

# Purposes / Tujuan
Welcome to "Natural Language Processing with Hugging Face Transformers,"

## Course Objectives / Objektif Course:
ENG:
This Guided Project will focus on text analysis tasks, which are:
- Text Classification.
- Sentiment Analysis. Classifies the polarity of a given text.
- Topic Classification. Classifies sequences into specified class names.
- Text Generator. Generates text from a given input.
- Token Classification.
- Name Entity Recognition (NER). Labels each word with the entity it represents.
- Question answering. Extracts the answer from the context.
- Text Summarization. Generates a summary of a long sequence of text or document.
- Translation. Translates text into another language.

IND:
Proyek Panduan ini akan fokus pada tugas analisis teks, yang meliputi:
- Klasifikasi Teks.
- Analisis Sentimen. Mengklasifikasikan polaritas dari teks yang diberikan.
- Klasifikasi Topik. Mengklasifikasikan urutan menjadi nama kelas yang ditentukan.
- Pembuat Teks. Menghasilkan teks dari masukan yang diberikan.
- Klasifikasi Token.
- Pengenalan Entitas Nama (NER). Memberi label setiap kata dengan entitas yang diwakilinya.
- Pertanyaan dan Jawaban. Mengekstrak jawaban dari konteks.
- Ringkasan Teks. Menghasilkan ringkasan dari urutan teks atau dokumen panjang.
- Penerjemahan. Menerjemahkan teks ke bahasa lain.

## Required Libraries / Library yang Diperlukan:
**Installing Required Libraries**

The following required libraries are pre-installed in the Skills Network Labs environment. However, if you run this notebook commands in a different Jupyter environment (e.g. Watson Studio or Anaconda), you will need to install these libraries by removing the # sign before !mamba in the code cell below.

```python
# All Libraries required for this lab are listed below. The libraries pre-installed on Skills Network Labs are commented.
# !mamba install -qy pandas==1.3.4 numpy==1.21.4 seaborn==0.9.0 matplotlib==3.5.0 scikit-learn==0.20.1
# Note: If your environment doesn't support "!mamba install", use "!pip install"
```

The following required libraries are not pre-installed in the Skills Network Labs environment. You will need to run the following cell to install them:
- `pip install torch`
- `pip install --upgrade torch`
- `pip install -q transformers`
- `pip install datasets evaluate transformers[sentencepiece]`
- `pip install sacremoses`

---

**Menginstal Perpustakaan yang Diperlukan**

Berikut adalah perpustakaan yang diperlukan yang sudah diinstal sebelumnya di lingkungan Skills Network Labs. Namun, jika Anda menjalankan perintah notebook ini di lingkungan Jupyter yang berbeda (misalnya, Watson Studio atau Anaconda), Anda perlu menginstal perpustakaan ini dengan menghapus tanda # sebelum !mamba dalam sel kode di bawah ini.

```python
# Semua perpustakaan yang diperlukan untuk praktikum ini tercantum di bawah. Perpustakaan yang diinstal sebelumnya di Skills Network Labs dikomentari.
# !mamba install -qy pandas==1.3.4 numpy==1.21.4 seaborn==0.9.0 matplotlib==3.5.0 scikit-learn==0.20.1
# Catatan: Jika lingkungan Anda tidak mendukung "!mamba install", gunakan "!pip install"
```

Berikut adalah perpustakaan yang diperlukan yang belum diinstal di lingkungan Skills Network Labs. Anda perlu menjalankan sel berikut untuk menginstalnya:
- `pip install torch`
- `pip install --upgrade torch`
- `pip install -q transformers`
- `pip install datasets evaluate transformers[sentencepiece]`
- `pip install sacremoses`
## Target Audience / Target Audiens:
ENG:
This course is suitable for AI enthusiasts, developers, and professionals seeking to enhance their skills in prompt engineering. It is ideal for those interested in leveraging OpenAI, Hugging Face, and Langchain for diverse AI applications.

IDN:
Kursus menggunakan kombinasi kuliah, latihan praktis, dan proyek dunia nyata untuk memastikan peserta mendapatkan pengalaman praktis dan pemahaman komprehensif tentang rekayasa cepat.
