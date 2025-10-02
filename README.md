
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















