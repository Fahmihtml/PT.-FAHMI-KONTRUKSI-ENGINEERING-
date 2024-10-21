<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bucin untuk Nong Ila</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #fce4ec;
            color: #880e4f;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        h1 {
            margin-bottom: 20px;
        }
        #message {
            font-size: 1.5rem;
            padding: 20px;
            border: 2px solid #ad1457;
            border-radius: 10px;
            width: 50%;
        }
    </style>
</head>
<body>

    <h1>Bucin untuk Nong Ila</h1>
    <div id="message">Nong Ila, kamu adalah alasan kenapa aku selalu tersenyum.</div>

    <script>
        const messages = [
            "Nong Ila, kamu adalah alasan kenapa aku selalu tersenyum.",
            "Setiap hariku dimulai dan berakhir dengan memikirkanmu.",
            "Kamu itu seperti bintang, selalu bersinar di hatiku, Nong Ila.",
            "Kalau aku punya satu harapan, itu adalah untuk selalu bersamamu, Nong Ila.",
            "Nong Ila, kamu seperti oksigen, aku tidak bisa hidup tanpamu.",
            "Bersamamu adalah saat-saat yang paling indah dalam hidupku, Nong Ila.",
            "Aku nggak butuh dunia yang besar, cukup ada kamu di sisiku, Nong Ila."
        ];

        let index = 0;
        const messageElement = document.getElementById('message');

        // Fungsi untuk mengganti pesan bucin setiap 3 detik
        function changeMessage() {
            index = (index + 1) % messages.length;
            messageElement.textContent = messages[index];
        }

        // Ganti pesan setiap 3 detik
        setInterval(changeMessage, 3000);
    </script>

</body>
</html>
