# Quizz
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quizz</title>
</head>
<body>
    <h1>Selamat Datang di Kuis</h1>
    <p>Pilih jawaban yang benar!</p>
</body>
</html>

<!DOCTYPE html>
<html>
<head>
    <title>Kuis Pengetahuan Umum</title>
    <script>
        function cekJawaban() {
            let skor = 0;

            // Mengambil jawaban yang dipilih
            let jawaban1 = document.querySelector('input[name="soal1"]:checked');
            let jawaban2 = document.querySelector('input[name="soal2"]:checked');
            let jawaban3 = document.querySelector('input[name="soal3"]:checked');
            let jawaban4 = document.querySelector('input[name="soal4"]:checked');
            let jawaban5 = document.querySelector('input[name="soal5"]:checked');

            // Memeriksa jawaban yang benar
            if (jawaban1 && jawaban1.value === "c") skor++;
            if (jawaban2 && jawaban2.value === "c") skor++;
            if (jawaban3 && jawaban3.value === "c") skor++;
            if (jawaban4 && jawaban4.value === "b") skor++;
            if (jawaban5 && jawaban5.value === "c") skor++;

            // Menampilkan hasil
            alert("Skor Anda: " + skor + "/5");
        }
    </script>
</head>
<body>
    <h2>Kuis Pengetahuan Umum</h2>
    
    <p>1. Ibukota dari negara Jepang adalah...</p>
    <input type="radio" name="soal1" value="a"> Beijing<br>
    <input type="radio" name="soal1" value="b"> Seoul<br>
    <input type="radio" name="soal1" value="c"> Tokyo<br>
    <input type="radio" name="soal1" value="d"> Bangkok<br>

    <p>2. Siapakah penemu bola lampu?</p>
    <input type="radio" name="soal2" value="a"> Nikola Tesla<br>
    <input type="radio" name="soal2" value="b"> Albert Einstein<br>
    <input type="radio" name="soal2" value="c"> Thomas Alva Edison<br>
    <input type="radio" name="soal2" value="d"> Isaac Newton<br>

    <p>3. Gunung tertinggi di dunia adalah...</p>
    <input type="radio" name="soal3" value="a"> Gunung Kilimanjaro<br>
    <input type="radio" name="soal3" value="b"> Gunung Elbrus<br>
    <input type="radio" name="soal3" value="c"> Gunung Everest<br>
    <input type="radio" name="soal3" value="d"> Gunung Fuji<br>

    <p>4. Planet mana yang dikenal sebagai 'Planet Merah'?</p>
    <input type="radio" name="soal4" value="a"> Venus<br>
    <input type="radio" name="soal4" value="b"> Mars<br>
    <input type="radio" name="soal4" value="c"> Jupiter<br>
    <input type="radio" name="soal4" value="d"> Saturnus<br>

    <p>5. Berapakah hasil dari 25 × 4?</p>
    <input type="radio" name="soal5" value="a"> 50<br>
    <input type="radio" name="soal5" value="b"> 75<br>
    <input type="radio" name="soal5" value="c"> 100<br>
    <input type="radio" name="soal5" value="d"> 125<br>

    <br><br>
    <button onclick="cekJawaban()">Submit</button>
</body>
</html>
