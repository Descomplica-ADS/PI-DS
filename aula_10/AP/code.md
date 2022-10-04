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
        <form id="getForm">
            <label for="nome">Nome</label>
            <input id="nome" name="nome" type="text">

            <label for="sobrenome">Sobrenome</label>
            <input id="sobrenome" name="sobrenome" type="text">

            <label for="email">E-mail</label>
            <input id="email" name="email" type="email">

            <div id="divResult">VALORES: -</div>

            <button type="button" onclick="calc()">Imprimir Valores</button>
        </form>
    </body>

    <script>
        function calc() {
            const form = document.getElementById('getForm')
            const div  = document.getElementById('divResult')

            const nome      = String(form.children.nome.value)
            const sobrenome = String(form.children.sobrenome.value)
            const email     = String(form.children.email.value)

            if (nome.length && sobrenome.length && email.length)
                return div.innerHTML = `VALORES: <br/><br/>${nome}<br/>${sobrenome}<br/>${email}`
        }
    </script>
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

    background-color: #100d1a;
    color: white;
    font-family: Arial, Helvetica, sans-serif;
    font-size: calc(0.7rem * 2);

    display: flex;
    align-items: center;
    justify-content: center;
}

form {
    width: 22rem;

    background-color: #ffffff0d;
    box-shadow: 1rem 1rem 2rem 0 #00000033, inset 0rem -20rem 17rem -19rem #962dff80;

    padding: 2rem;
    margin: 1rem;

    display: flex;
    flex-direction: column;

    border-radius: 1rem;

    overflow: hidden;
}
input {
    background-color: #ffffff1a;
    color: #ffffff80;
    font-size: 1rem;
    border: none;

    padding: 0.5rem 1rem;
    margin-bottom: 1rem;

    border-radius: 0.5rem;
}

#divResult {
    background-color: #962dff80;
    color: #b366ff;
    border: 0.15rem dashed #962dff;
    font-size: 1rem;
    font-weight: bold;
    text-align: center;
    line-height: 1.4rem;

    padding: 2rem 1rem;
    margin: 1.5rem 0;

    border-radius: 0.5rem;
}

button {
    background-color: #962dffb3;
    color: white;
    border: none;
    font-size: 0.9rem;
    font-weight: bold;
    letter-spacing: 0.03rem;
    text-transform: uppercase;

    padding: 0.7rem 1rem;

    transition: filter 0.3s;

    border-radius: 0.5rem;
}
button:hover { filter: opacity(0.8); }
```