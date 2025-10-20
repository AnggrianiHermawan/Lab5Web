# Praktikum 5: JavaScript

**Nama:** _Anggriani Hermawan_  
**NIM:** _312410175_  
**Kelas:** TI.24.A2 

---

## Langkah-langkah Praktikum

### 1. Persiapan
Buat folder baru dengan nama:
```
lab5_javascript
```
Lalu buat file:
```
lab5_javascript.html
```

---
### 2️. Pengenalan JavaScript

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```
Penjelasan:
- document.write() menampilkan teks langsung di halaman web.
- console.log() menampilkan teks di console browser (tekan F12 → Console).
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 180751" src="https://github.com/user-attachments/assets/2ef20749-27b0-44c4-8dfb-7355e848f124" />

### 3️. Menjalankan JavaScript dari File Eksternal

**File:** eksternal.js
```javascript
document.write("Hello World dari file eksternal!");
```

**File HTML:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Javascript Eksternal</title>
    <script src="eksternal.js"></script>
</head>
<body>
    <h1>Contoh JavaScript Eksternal</h1>
</body>
</html>
```
Penjelasan:
- File eksternal memisahkan JavaScript dari HTML agar kode lebih rapi.
- Tag <script src="eksternal.js"></script> digunakan untuk memanggil file JS.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 180841" src="https://github.com/user-attachments/assets/a2a40510-69a6-4e92-9048-5c0173f8f9cb" />

### 4️. Alert, Prompt, dan Function

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Alert, Prompt, dan Function</title>
    <script>
        window.onload = function() {
            alert("Selamat datang di halaman JavaScript!");
            var nama = prompt("Siapa nama kamu?");
            document.write("Hai, " + nama + "! Selamat belajar JavaScript.<br><br>");
        }
        function pesan() {
            alert("Ini pesan dari fungsi JavaScript!");
        }
    </script>
</head>
<body>
    <h2>Contoh Alert, Prompt, dan Function</h2>
    <button onclick="pesan()">Klik untuk melihat pesan</button>
</body>
</html>
```
Penjelasan:
- alert() menampilkan pop-up peringatan.
- prompt() meminta input pengguna.
- function digunakan untuk membuat blok kode yang dapat dipanggil.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 180922" src="https://github.com/user-attachments/assets/ac613a44-ff5d-47f5-b6a9-3e631274f297" />
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 180936" src="https://github.com/user-attachments/assets/767dec82-7acd-4d99-a48a-a6789594437b" />
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181002" src="https://github.com/user-attachments/assets/3fc3f637-a08b-449b-bce4-bef5e65ba4ee" />

### 5️. Operasi Dasar Aritmatika

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Operasi Aritmatika</title>
    <script>
        var a = 10;
        var b = 5;
        var hasil = a + b;
        document.write("Hasil penjumlahan: " + hasil);
    </script>
</head>
<body>
</body>
</html>
```
Penjelasan:
- JavaScript dapat melakukan operasi seperti +, -, *, /, dan %.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181053" src="https://github.com/user-attachments/assets/cbdab8b2-870a-471b-93e3-5f0bec6735d9" />

### 6. Seleksi Kondisi (if...else)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Seleksi Kondisi</title>
    <script>
        var nilai = prompt("Masukkan nilai ujian (0-100): ");
        if (nilai >= 60) {
            document.write("Selamat, Anda Lulus!");
        } else {
            document.write("Maaf, Anda Tidak Lulus.");
        }
    </script>
</head>
<body>
</body>
</html>
```
Penjelasan:
- if...else digunakan untuk pengambilan keputusan.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181240" src="https://github.com/user-attachments/assets/3ac8b835-265d-451b-9c74-15eeebc6a3ef" />
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181252" src="https://github.com/user-attachments/assets/d8a7ac74-e3a1-4319-9199-bd18a937fd36" />

### 7. Operator Switch

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Operator Switch</title>
    <script>
        var nilai = prompt("Masukkan nilai huruf (A–E):");
        switch (nilai.toUpperCase()) {
            case "A":
                document.write("Nilai Anda Sangat Baik");
                break;
            case "B":
                document.write("Nilai Anda Baik");
                break;
            case "C":
                document.write("Nilai Anda Cukup");
                break;
            case "D":
                document.write("Nilai Anda Kurang");
                break;
            case "E":
                document.write("Nilai Anda Sangat Kurang");
                break;
            default:
                document.write("Nilai tidak valid");
        }
    </script>
</head>
<body>
</body>
</html>
```
Penjelasan:
- switch cocok untuk banyak kondisi dengan pilihan tetap.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181416" src="https://github.com/user-attachments/assets/8772a087-d3e2-4c4d-906a-61c9c224a84b" />
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181432" src="https://github.com/user-attachments/assets/02d13c14-aef7-4c1d-a0c8-a3ee706f1f4a" />

### 8. Form Input

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Form Input</title>
    <script>
        function tampilkanNama() {
            let nama = document.getElementById("nama").value;
            alert("Halo, " + nama);
        }
    </script>
</head>
<body>
    <h2>Contoh Form Input</h2>
    <input type="text" id="nama" placeholder="Masukkan nama">
    <button onclick="tampilkanNama()">Tampilkan</button>
</body>
</html>
```
Penjelasan:
- getElementById digunakan untuk mengambil nilai dari elemen HTML berdasarkan ID.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181517" src="https://github.com/user-attachments/assets/7d6d7ecc-a5b5-4139-80bd-bb2a48929127" />
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181529" src="https://github.com/user-attachments/assets/4c1dd80e-9d53-4e49-8025-8ecba95ba35f" />

### 9. Validasi Form (Tugas Akhir)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Validasi Form</title>
    <script>
        function validasiForm() {
            let nama = document.forms["formku"]["nama"].value;
            let email = document.forms["formku"]["email"].value;
            let pesan = document.forms["formku"]["pesan"].value;

            if (nama == "" || email == "" || pesan == "") {
                alert("Semua kolom wajib diisi!");
                return false;
            }

            let pattern = /^[^ ]+@[^ ]+\.[a-z]{2,3}$/;
            if (!email.match(pattern)) {
                alert("Format email tidak valid!");
                return false;
            }

            alert("Form berhasil dikirim!");
            return true;
        }
    </script>
</head>
<body>
    <h2>Form Validasi</h2>
    <form name="formku" onsubmit="return validasiForm()">
        <p>Nama: <input type="text" name="nama"></p>
        <p>Email: <input type="text" name="email"></p>
        <p>Pesan: <textarea name="pesan" cols="30" rows="5"></textarea></p>
        <p>
            <input type="submit" value="Kirim">
            <input type="reset" value="Reset">
        </p>
    </form>
</body>
</html>
```
Penjelasan:
- Mengecek apakah input kosong.
- Mengecek format email dengan regex sederhana.
- Jika valid → menampilkan pesan sukses.
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181631" src="https://github.com/user-attachments/assets/27da7414-87ce-4e95-99bd-7a2ba48bfd62" />
<img width="1920" height="1080" alt="Cuplikan layar 2025-10-20 181645" src="https://github.com/user-attachments/assets/aa09bd6a-57c5-4366-a7e4-bc4980b83984" />

