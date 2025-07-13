**Data Scraping \& Preprocessing: Countries from scrapethissite.com**



1. Penjelasan Data



\- Sumber: \[Scrape This Site — Simple Countries Page](https://www.scrapethissite.com/pages/simple/)

-Fitur yang diambil:

* Name (nama negara)
* Capital (ibukota)
* Population (populasi)
* Area (luas wilayah)
* Jumlah data\*\*: 32 negara





2\. Proses Scraping



* Tools

\- Python

\- `requests` untuk mengambil HTML

\- `BeautifulSoup` untuk parsing dan ekstraksi data



* Flow



1. &nbsp;Mengirim request HTTP ke URL target  

2\.  Parse HTML menggunakan BeautifulSoup  

3\.  Ekstraksi informasi nama negara, ibukota, populasi, dan area  

4\.  Simpan data ke DataFrame pandas  





3\. Proses Preprocessing

1\. Tahapan



\- Konversi teks ke lowercase

\- Menghapus angka

\- Menghapus tanda baca

\- Menghapus stopwords (bahasa Inggris)

\- Stemming (Snowball Stemmer)



2\. Contoh Sebelum \& Sesudah

* Sebelum

Name: United Arab Emirates

Capital: Abu Dhabi

* Sesudah

Name: united arab emirate

Capital: abu dhabi



\## 💭 Refleksi Singkat



4\. Kendala



\- Beberapa website melarang scraping atau memberikan proteksi (seperti CAPTCHA atau Cloudflare).

\- Jika struktur HTML berubah, proses parsing gagal.



5\.  Solusi



\- Menggunakan header User-Agent saat scraping agar lebih aman.

\- Mengecek dan memperbarui selector CSS secara berkala.

\- Menyimpan hasil scraping ke file lokal sebelum preprocessing untuk mempermudah debugging.



