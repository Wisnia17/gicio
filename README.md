<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TO NIE KREDYT</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: rgb(93, 94, 107);
            color: #fff;
            text-align: center;
            padding: 20px;
        }

        aside {
            background-color: rgb(233, 54, 69);
            padding: 20px;
            float: left;
            width: 20%;
        }

        main {
            padding: 20px;
            float: left;
            width: 70%;
        }

        footer {
            clear: both;
            background-color: rgb(93, 94, 107);
            color: #fff;
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>TO NIE KREDYT</h1>
    </header>

    <aside>
        <h2>MENU</h2>
        <ul>
           <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
        </ul>
    </aside>
<center>
    <main>
        <h2>Witaj na naszej stronie!</h2>
        <p>Na naszej stronie swoje dane osobowe wpisujesz dobrowolnie i nie bierzemy odpowiedzialności jeśli stanie się coś złego xD. </p><br>
        <title>Formularz z Wyświetlaniem Danych</title>
    <style>
        label {
            display: block;
            margin-bottom: 10px;
        }

        input[type="text"], input[type="number"], input[type="email"], input[type="tel"] {
            width: 50%;
            padding: 10px;
            margin-bottom: 15px;
        }

        select {
            width: 50%;
            padding: 10px;
            margin-bottom: 15px;
        }

        button {
            padding: 10px 20px;
            background-color: #333;
            color: #fff;
            border: none;
            cursor: pointer;
        }

        #wyniki {
            border: 1px solid #ccc;
            padding: 20px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>TU WPISZ DANE STARY (:</h1>
    <form id="formularz">
        <label for="imie">Imię:</label>
        <input type="text" id="imie" name="imie" required>

        <label for="nazwisko">Nazwisko:</label>
        <input type="text" id="nazwisko" name="nazwisko" required>

        <label for="wiek">Ilość lat:</label>
        <input type="number" id="wiek" name="wiek" required>

        <label for="plec">Płeć:</label>
        <select id="plec" name="plec">
            <option value="mezczyzna">Mężczyzna</option>
            <option value="kobieta">Kobieta</option>
        </select>

        <label for="pesel">PESEL:</label>
        <input type="text" id="pesel" name="pesel" pattern="[0-9]{11}" title="Wprowadź 11 cyfr PESEL" required>

        <label for="telefon">Numer telefonu:</label>
        <input type="tel" id="telefon" name="telefon" pattern="[0-9]{9,15}" title="Wprowadź numer telefonu" required>

        <label for="adres">Miejsce zamieszkania:</label>
        <input type="text" id="adres" name="adres" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <button type="button" onclick="wyswietlDane()">Wyślij</button>
    </form>

    <div id="wyniki">
        <h2>Podsumowanie:</h2>
        <p>Imię: <span id="wynikImie"></span></p>
        <p>Nazwisko: <span id="wynikNazwisko"></span></p>
        <p>Ilość lat: <span id="wynikWiek"></span></p>
        <p>Płeć: <span id="wynikPlec"></span></p>
        <p>PESEL: <span id="wynikPesel"></span></p>
        <p>Numer telefonu: <span id="wynikTelefon"></span></p>
        <p>Miejsce zamieszkania: <span id="wynikAdres"></span></p>
        <p>Email: <span id="wynikEmail"></span></p>
    </div>

    <script>
        function wyswietlDane() {
            const imie = document.getElementById("imie").value;
            const nazwisko = document.getElementById("nazwisko").value;
            const wiek = document.getElementById("wiek").value;
            const plec = document.getElementById("plec").value;
            const pesel = document.getElementById("pesel").value;
            const telefon = document.getElementById("telefon").value;
            const adres = document.getElementById("adres").value;
            const email = document.getElementById("email").value;

            document.getElementById("wynikImie").textContent = imie;
            document.getElementById("wynikNazwisko").textContent = nazwisko;
            document.getElementById("wynikWiek").textContent = wiek;
            document.getElementById("wynikPlec").textContent = plec;
            document.getElementById("wynikPesel").textContent = pesel;
            document.getElementById("wynikTelefon").textContent = telefon;
            document.getElementById("wynikAdres").textContent = adres;
            document.getElementById("wynikEmail").textContent = email;
        }
    </script>
    </main>
</center>
    <footer>
        &copy; 2023 TO NIE KREDYT | by lenok
    </footer>
</body>
</html>
