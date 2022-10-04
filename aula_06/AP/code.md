**R e s p o s t a - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -**

*HTML:*
```html
<!DOCTYPE html>
<html lang="pt-BR">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">

        <title>Pratica Integradora Desenvolvimento de Software</title>

        <link type="text/css" rel="stylesheet" href="css/estilo.css">
    </head>
    <body>
        <h2>Fundamentos sobre estilos</h2>

        <table>
            <thead>
                <tr>
                    <th>Dia</th>
                    <th>Tempo</th>
                    <th>Mínima</th>
                    <th>Máxima</th>
                </tr>
            </thead>

            <tbody>
                <tr>
                    <td>Domingo</td>
                    <td>🌨</td>
                    <td>-2°</td>
                    <td>9°</td>
                </tr>
                <tr>
                    <td>Segunda</td>
                    <td>⛈</td>
                    <td>8°</td>
                    <td>19°</td>
                </tr>
                <tr>
                    <td>Terça</td>
                    <td>🌥</td>
                    <td>10°</td>
                    <td>23°</td>
                </tr>
                <tr>
                    <td>Quarta</td>
                    <td>⛅</td>
                    <td>20°</td>
                    <td>26°</td>
                </tr>
                <tr>
                    <td>Quinta</td>
                    <td>🌤</td>
                    <td>21°</td>
                    <td>27°</td>
                </tr>
                <tr>
                    <td>Sexta</td>
                    <td>🌤</td>
                    <td>26°</td>
                    <td>32°</td>
                </tr>
                <tr>
                    <td>Sábado</td>
                    <td>🌤</td>
                    <td>28°</td>
                    <td>35°</td>
                </tr>
            </tbody>
        </table>
    </body>
</html>
```

*CSS:*
```css
* {
    margin: 0;
    padding: 0;

    box-sizing: border-box;
}

body {
    width: 100vw;
    height: 100vh;

    background-color: burlywood;
    color: white;
    font-family: Arial, Helvetica, sans-serif;
    font-size: calc(1rem * 2);

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
}

h2 { color: brown; }

table {
    background-color: blueviolet;
    color: white;
    border-collapse: collapse;

    margin: 0 1rem;

    display: flex;
    flex-direction: column;

    border-radius: 1rem;

    overflow: hidden;
}

thead {
    background-color: brown;
    color: coral;
    text-transform: uppercase;
    text-align: center;
}

tbody {
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
}
tbody tr:nth-child(even) { background-color: #ffffff1a; }

tr {
    padding: 0.5rem 1.5rem;

    display: flex;
    align-items: center;
}
td { width: 10rem; }
th { width: 100%; }
td, th { text-align: center; }
```