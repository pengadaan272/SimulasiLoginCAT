<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
    <style>
        /* Menghapus margin dan padding default pada body */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Times New Roman', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(5, 5, 255, 0.651); /* Background biru transparan */
        }

        /* Menyusun kontainer menggunakan Flexbox */
        .container {
            display: flex;
            justify-content: center; /* Mengatur gambar ke tengah secara horizontal */
            align-items: center; /* Mengatur gambar ke tengah secara vertikal */
        }

        .login-container {
            background: rgb(135, 206, 235); /* Warna biru langit */
            padding: 40px;
            border-radius: 7px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px; /* Menambahkan lebar maksimum */
        }

        h1 {
            font-size: 3em;
            color: #000000; /* Warna hitam */
            text-align: center;
            font-family: 'Consolas', monospace;
            font-weight: bolder;
            margin-bottom: 20px;
        }

        h2 {
            color: #000000; /* Warna hitam */
            text-align: center;
            font-family: 'Consolas', monospace;
            font-weight: lighter;
            margin-bottom: 10px;
        }

        .form-group {
            margin-bottom: 15px;
        }

        label {
            display: block;
            margin-bottom: 5px;
        }

        input[type="text"],
        input[type="password"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }

        input[type="submit"] {
            width: 100%;
            padding: 10px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 3px;
            cursor: pointer;
        }

        input[type="submit"]:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h1>Simulasi CAT</h1>
        <h2>Computer Assisted Test</h2>
        <h2>CAT</h2>
        <div class="container">
            <img src="https://cat.bkn.go.id/assets/img/logocat.png" alt="Gambar Eksternal" width="200" height="200">
        </div>
        <form action="https://cat.bkn.go.id/simulasi/" method="post">
            <div class="form-group">
                <label for="NIK">NIK:</label>
                <input type="text" id="NIK" name="NIK" required>
            </div>
            <div class="form-group">
                <label for="no_peserta">NO. PESERTA:</label>
                <input type="text" id="no_peserta" name="no_peserta" required>
            </div>
            <div class="form-group">
                <label for="pin_peserta">PIN. PESERTA:</label>
                <input type="password" id="pin_peserta" name="pin_peserta" required>
            </div>
            <div class="form-group">
                <label for="pin_sesi">PIN. SESI:</label>
                <input type="text" id="pin_sesi" name="pin_sesi" required>
            </div>
            <input type="submit" value="Masuk">
        </form>
    </div>
</body>
</html>
