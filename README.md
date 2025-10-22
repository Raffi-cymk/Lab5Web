# Lab5Web

🎯 Tujuan Praktikum

1. Mahasiswa mampu memahami sintaks dasar JavaScript.

2. Mahasiswa mampu memahami penggunaan JavaScript di halaman web.

3. Mahasiswa mampu membuat kode JavaScript sederhana.

4. Mahasiswa mampu memanipulasi elemen HTML dengan JavaScript.

---

💻 File & Struktur Folder

📂 Folder: lab5_javascript/
📄 File di dalamnya:

lab5_javascript.html → file utama HTML

eksternal.js → file JavaScript eksternal

---

⚙️ Langkah-langkah Praktikum & Screenshot (1–17)
📸 1. Kodingan JavaScript awal (dengan eksternal.js)

Menunjukkan struktur awal HTML dan cara menghubungkan file JavaScript eksternal:
<script type="text/javascript" src="eksternal.js"></script>
📍Fungsi: memisahkan script dari HTML agar rapi dan mudah dikelola.

📸 2. Kodingan file eksternal.js

Isi file:
document.write("Hello World dari file eksternal!");
📍Fungsi: menampilkan teks langsung ke halaman dari file eksternal.

📸 3. Tampilan halaman web pertama

Menampilkan teks:
Hello World Hello World dari file eksternal!
📍Artinya script internal dan eksternal sama-sama berjalan.

📸 4. Kodingan versi lanjut (dengan tombol “Klik Aku!”)

Isi fungsi baru:
function sapa() {
  alert("Halo dunia dari fungsi!");
}

dan tombol HTML:
<button onclick="sapa()">Klik Aku!</button>
📍Menunjukkan penerapan fungsi dan event onclick di JavaScript.

📸 5. Tampilan web dengan tombol “Klik Aku!”

📍Menampilkan hasil dari fungsi di browser — ketika tombol diklik, muncul alert “Halo dunia dari fungsi!”

📸 6. Kodingan dengan prompt & if–else (Masukkan nilai kamu)

Isi:
let nilai = prompt("Masukkan nilai kamu:");
if (nilai >= 60) {
  alert("Kamu LULUS!");
} else {
  alert("Kamu BELUM LULUS!");
}
📍Fungsi: menggunakan seleksi kondisi (if–else) untuk menilai input pengguna.

📸 7. Tampilan hasil if–else (alert “Kamu BELUM LULUS!”)

📍Menunjukkan program berjalan sesuai kondisi (nilai < 60).

📸 8. Kodingan switch–case (Masukkan angka 1–3)

Isi:
let hari = prompt("Masukkan angka 1-3:");
switch(hari) {
  case "1": alert("Senin"); break;
  case "2": alert("Selasa"); break;
  case "3": alert("Rabu"); break;
  default: alert("Hari tidak dikenal");
}
📍Fungsi: menerapkan percabangan multi-kondisi dengan switch.

📸 9. Prompt input angka “1”

📍Menunjukkan pengguna diminta memasukkan angka untuk menentukan hari.

📸 10. Hasil alert: “Senin”

📍Output sesuai input angka “1”.

📸 11. Prompt input angka “2”

📍Mengetes kondisi kedua pada switch case.

📸 12. Hasil alert: “Selasa”

📍Output sesuai input angka “2”.

📸 13. Prompt input angka “3”

📍Mengetes kondisi ketiga pada switch case.

📸 14. Hasil alert: “Rabu”

📍Output sesuai input angka “3”.

📸 15. Prompt input angka “0”

📍Mengetes kondisi di luar case yang tersedia.

📸 16. Hasil alert: “Hari tidak dikenal”

📍Berhasil menunjukkan case default dijalankan jika input tidak sesuai.

📸 17. Hasil Validasi HTML di validator.w3.org

📍Setelah perbaikan struktur HTML:
<meta charset="UTF-8">
dan penghapusan <head> ganda, hasilnya:
✅ No errors found
⚠️ (hanya warning minor yang bisa diabaikan)
