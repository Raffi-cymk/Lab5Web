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

![Screenshot 2025-10-22 105203.png](https://github.com/Raffi-cymk/Lab5Web/edit/main/README.md)

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


---

📋 Kodingan Akhir (Final Version)
Berikut struktur HTML lengkap yang sudah valid:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Mengenal JavaScript</title>
    <script type="text/javascript" src="eksternal.js"></script>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>

    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>

    <script>
        let nama = prompt("Siapa namamu?");
        document.write("Halo, " + nama + "!");
    </script>

    <script>
        function sapa() {
            alert("Halo dunia dari fungsi!");
        }
    </script>

    <button onclick="sapa()">Klik Aku!</button>

    <script>
        let nilai = prompt("Masukkan nilai kamu:");
        if (nilai >= 60) {
            alert("Kamu LULUS!");
        } else {
            alert("Kamu BELUM LULUS!");
        }
    </script>

    <script>
        let hari = prompt("Masukkan angka 1-3:");
        switch(hari) {
            case "1": alert("Senin"); break;
            case "2": alert("Selasa"); break;
            case "3": alert("Rabu"); break;
            default: alert("Hari tidak dikenal");
        }
    </script>
</body>
</html>

---

🧠 Kesimpulan

* JavaScript dapat menampilkan teks, pesan, dan interaksi di halaman web.

* Kode dapat ditempatkan di internal HTML atau file eksternal .js.

* Penggunaan alert(), prompt(), if–else, switch, dan function telah berhasil diterapkan.

* Struktur HTML sudah valid (no error) di validator W3C.

---

❓ Pertanyaan & Jawaban Praktikum

> Pertanyaan:
1️⃣ Buat script untuk melakukan validasi pada isian form.

✅ Jawaban Contoh Validasi Form:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Validasi Form</title>
    <script>
        function validateForm() {
            let nama = document.forms["myForm"]["nama"].value;
            if (nama === "") {
                alert("Nama harus diisi!");
                return false;
            }
        }
    </script>
</head>
<body>
    <h2>Form Validasi</h2>
    <form name="myForm" onsubmit="return validateForm()">
        Nama: <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>
</body>
</html>

📍Fungsi: mengecek apakah kolom “Nama” diisi sebelum form dikirim.
