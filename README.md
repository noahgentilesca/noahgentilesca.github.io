<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menüplan</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        header {
            text-align: center;
            margin-bottom: 40px;
        }
        img.logo {
            width: 200px;
            margin-top: 20px;
        }
        #uhrzeit {
            font-size: 20px;
            margin-top: 10px;
            color: #555;
        }
        table {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            border-collapse: collapse;
        }
        th, td {
            padding: 15px;
            border: 1px solid #ddd;
            text-align: center;
        }
        th {
            background-color: #007BFF;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f9f9f9;
        }
    </style>
</head>
<body>

<header>
    <img src="btc_jost_logo.png" alt="BTC.jost AG Logo" class="logo">
    <h1>BTC.jost AG - Wochen-Menüplan</h1>
    <p>Gültig vom 04.03.2025 bis 10.03.2025</p>
    <div id="uhrzeit">Aktuelle Uhrzeit: --:--:--</div>
</header>

<table>
    <tr>
        <th>Tag</th>
        <th>Datum</th>
        <th>Uhrzeit</th>
        <th>Menü</th>
    </tr>
    <tr>
        <td>Montag</td>
        <td>04.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Spaghetti Bolognese mit Salat</td>
    </tr>
    <tr>
        <td>Dienstag</td>
        <td>05.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Schnitzel mit Pommes und Gemüse</td>
    </tr>
    <tr>
        <td>Mittwoch</td>
        <td>06.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Gemüsecurry mit Reis</td>
    </tr>
    <tr>
        <td>Donnerstag</td>
        <td>07.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Pizza Margherita</td>
    </tr>
    <tr>
        <td>Freitag</td>
        <td>08.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Fischstäbchen mit Kartoffelpüree</td>
    </tr>
    <tr>
        <td>Samstag</td>
        <td>09.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Chickenburger mit Pommes</td>
    </tr>
    <tr>
        <td>Sonntag</td>
        <td>10.03.2025</td>
        <td>12:00 - 13:00</td>
        <td>Schweinsbraten mit Knödeln</td>
    </tr>
</table>

<script>
    function updateUhrzeit() {
        const jetzt = new Date();
        const stunden = jetzt.getHours().toString().padStart(2, '0');
        const minuten = jetzt.getMinutes().toString().padStart(2, '0');
        const sekunden = jetzt.getSeconds().toString().padStart(2, '0');
        document.getElementById('uhrzeit').textContent = `Aktuelle Uhrzeit: ${stunden}:${minuten}:${sekunden}`;
    }
    setInterval(updateUhrzeit, 1000);
    updateUhrzeit();
</script>

</body>
</html>
