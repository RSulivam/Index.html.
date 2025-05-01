# Index.html.
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Teste CORS</title>
</head>
<body>
    <h1>Teste CORS Gojek</h1>
    <p>Se você está vendo esta página, o GitHub Pages está funcionando!</p>
    <script>
        fetch('https://developer.gojek.com', {
            method: 'GET',
            mode: 'cors'
        })
        .then(response => {
            document.body.innerHTML += '<p>Resposta: ' + response.status + '</p>';
        })
        .catch(error => {
            document.body.innerHTML += '<p>Erro: ' + error + '</p>';
        });
    </script>
</body>
</html>
