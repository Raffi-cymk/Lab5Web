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

<img width="1366" height="768" alt="Screenshot 2025-10-22 105203" src="https://github.com/user-attachments/assets/f0075fd8-7575-4b9a-8deb-183cfa7860a8" />


📸 2. Kodingan file eksternal.js

Isi file:
document.write("Hello World dari file eksternal!");
📍Fungsi: menampilkan teks langsung ke halaman dari file eksternal.

<img width="1366" height="768" alt="Screenshot 2025-10-22 105429" src="https://github.com/user-attachments/assets/c13dd9ba-9dba-4b59-8b38-94f24fd9db77" />

📸 3. Tampilan halaman web pertama

Menampilkan teks:
Hello World Hello World dari file eksternal!
📍Artinya script internal dan eksternal sama-sama berjalan.

<img width="1366" height="768" alt="Screenshot 2025-10-22 105545" src="https://github.com/user-attachments/assets/d42a075a-59e8-495c-a7fd-77b95293da03" />

📸 4. Kodingan versi lanjut (dengan tombol “Klik Aku!”)

Isi fungsi baru:
function sapa() {
  alert("Halo dunia dari fungsi!");
}

dan tombol HTML:
<button onclick="sapa()">Klik Aku!</button>
📍Menunjukkan penerapan fungsi dan event onclick di JavaScript.

<img width="1366" height="768" alt="Screenshot 2025-10-22 110312" src="https://github.com/user-attachments/assets/86014aec-8851-48af-be36-42371a906041" />

📸 5. Tampilan web dengan tombol “Klik Aku!”

📍Menampilkan hasil dari fungsi di browser — ketika tombol diklik, muncul alert “Halo dunia dari fungsi!”

<img width="1366" height="768" alt="Screenshot 2025-10-22 110516" src="https://github.com/user-attachments/assets/bdb19668-ddc7-49b1-8cdc-4bed74b82b36" />

📸 6. Kodingan dengan prompt & if–else (Masukkan nilai kamu)

Isi:
let nilai = prompt("Masukkan nilai kamu:");
if (nilai >= 60) {
  alert("Kamu LULUS!");
} else {
  alert("Kamu BELUM LULUS!");
}
📍Fungsi: menggunakan seleksi kondisi (if–else) untuk menilai input pengguna.

<img width="1366" height="768" alt="Screenshot 2025-10-22 110717" src="https://github.com/user-attachments/assets/9c474c2e-100c-49fb-a7db-cbca137aba87" />

📸 7. Tampilan hasil if–else (alert “Kamu BELUM LULUS!”)

<img width="1366" height="768" alt="Screenshot 2025-10-22 110822" src="https://github.com/user-attachments/assets/edc3c8b6-9bc2-466e-8ce3-171e2a0fab12" />

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

<img width="1366" height="768" alt="Screenshot 2025-10-22 111057" src="https://github.com/user-attachments/assets/42f2fc01-83ef-406b-a654-2f84a0c413d3" />

📸 9. Prompt input angka “1”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111410" src="https://github.com/user-attachments/assets/68ee5567-878e-4457-8de3-d665a297af82" />

📍Menunjukkan pengguna diminta memasukkan angka untuk menentukan hari.

📸 10. Hasil alert: “Senin”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111428" src="https://github.com/user-attachments/assets/7fc0f4cc-d02c-444d-8455-508cb9c576df" />

📍Output sesuai input angka “1”.

📸 11. Prompt input angka “2”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111518" src="https://github.com/user-attachments/assets/ab3812c1-2f42-4e5c-a7ca-881d41ade0b7" />

📍Mengetes kondisi kedua pada switch case.

📸 12. Hasil alert: “Selasa”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111536" src="https://github.com/user-attachments/assets/3f6b7339-7d15-45e9-b6c0-6f2e02e52024" />

📍Output sesuai input angka “2”.

📸 13. Prompt input angka “3”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111607" src="https://github.com/user-attachments/assets/515f16fa-fadb-447d-a809-e3f19366a71e" />

📍Mengetes kondisi ketiga pada switch case.

📸 14. Hasil alert: “Rabu”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111626" src="https://github.com/user-attachments/assets/1cffc3a5-caa0-4721-a37d-40f9abfbdfb2" />

📍Output sesuai input angka “3”.

📸 15. Prompt input angka “0”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111920" src="https://github.com/user-attachments/assets/50e492a0-ac05-4931-9ab0-db2c182cca22" />

📍Mengetes kondisi di luar case yang tersedia.

📸 16. Hasil alert: “Hari tidak dikenal”

<img width="1366" height="768" alt="Screenshot 2025-10-22 111933" src="https://github.com/user-attachments/assets/5718d498-9ab7-454a-a35f-3de51f885b52" />

📍Berhasil menunjukkan case default dijalankan jika input tidak sesuai.

📸 17. Hasil Validasi HTML di validator.w3.org

<img width="1366" height="768" alt="Screenshot 2025-10-22 115831" src="https://github.com/user-attachments/assets/73335c57-261e-4a35-b507-d7a91ce8b734" />

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
