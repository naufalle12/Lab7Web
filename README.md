# Lab7Web
Program sederhana php 
<!DOCTYPE html>
<html>
<head>
    <title>Form Input PHP</title>
</head>
<body>
    <h1>Form Input Data</h1>
    <form method="POST" action="">
        <label for="name">Nama:</label>
        <input type="text" id="name" name="name" required><br><br>

        <label for="birthdate">Tanggal Lahir:</label>
        <input type="date" id="birthdate" name="birthdate" required><br><br>

        <label for="job">Pekerjaan:</label>
        <select id="job" name="job" required>
            <option value="Programmer">Programmer</option>
            <option value="Desainer">Desainer</option>
            <option value="Manajer">Manajer</option>
        </select><br><br>

        <input type="submit" value="Submit">
    </form>

    <?php
    if ($_SERVER["REQUEST_METHOD"] == "POST") {
        // Mengambil data dari form
        $name = $_POST['name'];
        $birthdate = $_POST['birthdate'];
        $job = $_POST['job'];

        // Menghitung umur
        $birthDateObj = new DateTime($birthdate);
        $today = new DateTime();
        $age = $today->diff($birthDateObj)->y;

        // Menentukan gaji berdasarkan pekerjaan
        $salary = 0;
        switch ($job) {
            case "Programmer":
                $salary = 8000000;
                break;
            case "Desainer":
                $salary = 6000000;
                break;
            case "Manajer":
                $salary = 12000000;
                break;
        }

        // Menampilkan output
        echo "<h2>Hasil Input:</h2>";
        echo "Nama: $name<br>";
        echo "Tanggal Lahir: $birthdate<br>";
        echo "Umur: $age tahun<br>";
        echo "Pekerjaan: $job<br>";
        echo "Gaji: Rp " . number_format($salary, 0, ',', '.') . "<br>";
    }
    ?>
</body>
</html>
![Screenshot (318)](https://github.com/user-attachments/assets/d95ca924-132c-4c9d-ba64-dcbb0ff12342)
# file xampp
![Screenshot (301)](https://github.com/user-attachments/assets/f30af18c-19bd-4aad-9486-4e7f16f7e806)
# konfigurasi pache
![Screenshot (303)](https://github.com/user-attachments/assets/a00b51e6-8708-4fd2-bbcb-77e26b8115fd)
# konfigurasi mysql
![Screenshot (304)](https://github.com/user-attachments/assets/0bd2110a-b1f0-482b-b8e4-ecaaa20ed7fa)

## menjalankan web server
![Screenshot (301)](https://github.com/user-attachments/assets/bbbd2994-4cce-4335-8735-3e02643ce30e)
# test web server
![Screenshot (306)](https://github.com/user-attachments/assets/9aaebbb7-f31c-49d7-ae18-3d0b8f39af38)
# memulai php
![Screenshot (302)](https://github.com/user-attachments/assets/4b57bcfa-d931-457c-ac38-00b2c4f48b4b)
# akses direktori
![Screenshot (307)](https://github.com/user-attachments/assets/6a40aec4-b777-4e41-acac-b8d2e583f545)
# php dasar awal
![Screenshot (308)](https://github.com/user-attachments/assets/4701f56f-8885-4e22-8a8b-c24a7bf2074e)
# variable awal php
![Screenshot (309)](https://github.com/user-attachments/assets/3498d9ad-88c4-4761-b606-1981d7ecbd29)
# predefine variable
![Screenshot (310)](https://github.com/user-attachments/assets/9e938b2e-b202-492e-9c41-dd91777ff6ed)
# crate form input
![Screenshot (311)](https://github.com/user-attachments/assets/2a9d4ccd-1533-4a8a-9ce1-1badab37cd3e)
# operator
![Screenshot (312)](https://github.com/user-attachments/assets/3e71e036-4f02-4dcd-9150-16f6ac3f4407)
# kondisi if 
![Screenshot (313)](https://github.com/user-attachments/assets/5ea022ec-4ae3-4d35-85b6-848f8eff2a4d)
# kondisi switch
![Screenshot (314)](https://github.com/user-attachments/assets/adef2e4f-945c-4b51-8080-22bb94bef679)
# perulangan for
![Screenshot (315)](https://github.com/user-attachments/assets/e548bc8f-f491-4d14-a32d-47fbf933b7e4)
# perulangan while
![Screenshot (316)](https://github.com/user-attachments/assets/b62724c9-1530-416e-9cd0-e11c9b5ad6c6)
# perulanhgan dowhile
![Screenshot (317)](https://github.com/user-attachments/assets/dafaf90a-8d63-41c5-ae65-8a9ea3e61392)

Naufal Putra Ramadhan
312310052
TI.23.A1
