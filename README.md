<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jurnal Harian</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: #f4f4f9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
        }
        input, button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            font-size: 1em;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: #3498db;
            color: white;
            cursor: pointer;
        }
        h2 {
            text-align: center;
        }
        .content {
            display: none;
        }
        .content p {
            font-size: 1.2em;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Masukkan Password</h2>
    <div id="loginForm">
        <input type="password" id="password" placeholder="Password" required>
        <button onclick="checkPassword()">Masuk</button>
        <p id="error" style="color:red; display:none;">Password salah, coba lagi!</p>
    </div>

    <div id="content" class="content">
        <h2>📝 Jurnal Harian Saya</h2>
        <p><strong>18 April 2025:</strong> Hari ini aku merasa lebih tenang setelah jogging pagi. Langit cerah dan aku sempat merenung di taman selama 30 menit. 🌤️</p>
        <p><strong>17 April 2025:</strong> Hujan deras membuatku malas keluar rumah, jadi aku habiskan waktu dengan baca buku dan ngopi hangat. ☕📚</p>
    </div>
</div>

<script>
    function checkPassword() {
        var password = document.getElementById('password').value;
        var correctPassword = 'rahasia123';  // Ganti dengan password kamu
        var errorElement = document.getElementById('error');
        
        if (password === correctPassword) {
            document.getElementById('loginForm').style.display = 'none';
            document.getElementById('content').style.display = 'block';
        } else {
            errorElement.style.display = 'block';
        }
    }
</script>

</body>
</html># jurnal-harian
