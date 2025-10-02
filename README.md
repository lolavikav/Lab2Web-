
# Nama : Lola Seftyliani 
# Nim : 312410339
# Kelas : TI.24.A.4
# Matkul: Pemograman Web 1

# Lab2Web - Praktikum 2: CSS Dasar
## Langkah Praktikum
## 1. Membuat dokumen HTML
Pertama kita buat file baru `lab2_css_dasar.html.` Di dalamnya ditulis struktur HTML dasar berisi header, nav, dan div intro. Tujuannya agar ada konten yang nanti bisa kita beri style dengan CSS.
<img width="1266" height="895" alt="1" src="https://github.com/user-attachments/assets/8b0f6eaa-6353-4ad7-b4b3-e0bc75538307" />
Output:
<img width="1068" height="449" alt="11" src="https://github.com/user-attachments/assets/0f2b3311-1b26-4f12-9c72-0a8b58d446ff" />
## 2. Mendeklarasikan CSS internal
CSS internal ditulis di dalam tag `<style>` pada bagian `<head>`. Misalnya mengatur font, warna teks, ukuran heading, dan style tambahan untuk judul. Dengan internal CSS, semua elemen yang sesuai aturan akan langsung berubah tampilannya.
<img width="1510" height="2116" alt="2" src="https://github.com/user-attachments/assets/45875308-7a8c-4263-acbd-1b94637ddaa1" />
output:
<img width="1142" height="489" alt="22" src="https://github.com/user-attachments/assets/948c8da5-0d0a-4756-a4bf-d4f55fcdc7dc" />
## Menambahkan inline CSS
Inline CSS ditulis langsung di dalam tag HTML menggunakan atribut `style`. Contohnya di `<p style="text-align: center; color: #ccd8e4;"> ... </p>`. Hasilnya hanya berlaku untuk elemen tersebut saja. Inline CSS punya prioritas paling tinggi dibanding internal atau eksternal.
<img width="2142" height="444" alt="code" src="https://github.com/user-attachments/assets/60b575f8-707d-4f06-b12d-cce837943616" />
Output:
<img width="1514" height="478" alt="33" src="https://github.com/user-attachments/assets/1c1ecc53-9ac2-4dd8-9f3d-e4288a5fe8f2" />
## 4. Membuat CSS eksternal 
Buat file baru bernama `style_eksternal.css.` Isi file ini dengan aturan CSS, misalnya untuk `nav`, `a`, dan tampilan tombol. Lalu file CSS ini dipanggil ke HTML dengan tag `<link` `rel="stylesheet" href="style_eksternal.css">`.
<img width="710" height="862" alt="code 11" src="https://github.com/user-attachments/assets/26e495e0-f318-4305-9015-d95414eca3bd" />
<img width="1312" height="406" alt="code 12" src="https://github.com/user-attachments/assets/7c868b38-26c0-43bf-9c7f-8840a7dc8dce" />
Output:
<img width="884" height="603" alt="44" src="https://github.com/user-attachments/assets/52c0e5f8-a22d-4aff-a924-f9cbfbf0ae6a" />
## Menambahkan CSS Selector
Selector dipakai untuk memilih elemen tertentu.
- ID Selector `(#id)` → hanya berlaku untuk satu elemen dengan id tertentu.
- Class Selector `(.class)` → bisa dipakai di banyak elemen.
- <img width="772" height="1318" alt="code 14" src="https://github.com/user-attachments/assets/24f23eae-21f1-43dc-864f-1bc8c59f18f7" />
Output:
<img width="881" height="668" alt="55" src="https://github.com/user-attachments/assets/f42ba254-846c-4648-9047-c13623bae03a" />
## Pertanyaan dan Tugas 
## 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
Saya mencoba menambahkan beberapa properti CSS, contohnya:
Penjelasan:
<img width="1572" height="1508" alt="code 15" src="https://github.com/user-attachments/assets/29451ccd-a6bf-4397-bfbb-3fbad0c7916b" />
Output
<img width="887" height="217" alt="Screenshot 2025-10-02 234957" src="https://github.com/user-attachments/assets/4bcb9297-88d3-4a23-bace-6bc0f8d947c8" />
Penjelasan:
- Body: diberi background biru muda (#f0f8ff) dan font diganti dengan Arial supaya tampilan lebih modern.
- Heading (h1): diatur agar berwarna biru tua, posisinya rata tengah, hurufnya otomatis menjadi kapital semua, dan jarak antar huruf dibuat lebih lebar agar terlihat tegas.
- Paragraf (p) dibuat berwarna abu-abu gelap, rata tengah, huruf agak besar (18px), dan bergaya miring agar berbeda dengan teks judul.
Dengan pengaturan ini, teks “Halo, nama saya Fira” tampil lebih jelas dan menarik, serta memberikan contoh nyata bagaimana CSS dapat mengubah tampilan halaman web hanya dengan beberapa baris kode.
## 2.Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
Penjelasan:
<img width="891" height="753" alt="Screenshot 2025-10-02 235538" src="https://github.com/user-attachments/assets/d895c1a5-fc50-4ce7-99b3-7fba0d6bd282" />
Output:
<img width="882" height="261" alt="Screenshot 2025-10-02 235515" src="https://github.com/user-attachments/assets/c5edf45b-dfc7-4de0-a707-2673454e2564" />
Penjelasan:
Deklarasi `h1[...]` adalah aturan CSS yang berlaku untuk semua elemen `<h1>` pada halaman web, tanpa memandang letaknya. Jadi jika ada lima buah heading `<h1>` di halaman, maka semuanya akan terkena style yang sama. Aturan ini bersifat global untuk elemen tertentu.
Sementara itu, deklarasi `#intro h1 {...}` jauh lebih spesifik. Aturan ini hanya berlaku untuk elemen `<h1>` yang berada di dalam elemen lain yang memiliki atribut `id="intro"`. Artinya, jika ada beberapa heading `<h1>` di halaman, hanya `<h1>` yang berada di dalam `<div id="intro">...</div>` saja yang akan menerima style tersebut, sedangkan `<h1>` lainnya tidak terpengaruh.
## 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
Penjelasan:

Dalam CSS terdapat konsep yang disebut specificity (tingkat kekuatan aturan). Browser memiliki urutan prioritas dalam membaca style, yaitu:

Eksternal CSS → ditulis dalam file terpisah (.css) dan dipanggil dengan <link>.
Internal CSS → ditulis di dalam file HTML pada tag <style> dalam <head>.
Inline CSS → ditulis langsung dalam atribut style pada elemen HTML.
Jika ketiga jenis CSS tersebut diterapkan pada elemen yang sama, maka browser akan menampilkan style dari inline CSS, karena memiliki prioritas tertinggi. Internal CSS akan menimpa eksternal, sedangkan inline akan menimpa keduanya.
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )
Penjelasan Hasil:

Paragraf pertama (class="text-paragraf") → tampil merah.
Paragraf kedua (id="paragraf-1") → tampil biru.
Paragraf ketiga (id="paragraf-1" class="text-paragraf") → tetap biru, karena aturan ID selector lebih kuat daripada class selector.














