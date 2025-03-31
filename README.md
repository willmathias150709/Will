<!DOCTYPE html><html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PiraNarg's</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; }
        .produto { display: inline-block; margin: 20px; border: 1px solid #ddd; padding: 10px; }
        .produto img { width: 150px; height: 150px; }
        .botao { background: green; color: white; padding: 10px; border: none; cursor: pointer; }
    </style>
</head>
<body>
    <h1>Bem-vindo à PiraNarg's!</h1>
    <div id="produtos">
        <div class="produto">
            <img src="https://via.placeholder.com/150" alt="Produto 1">
            <h2>Produto 1</h2>
            <p>R$ 50,00</p>
            <button class="botao" onclick="adicionarAoCarrinho('Produto 1', 50)">Comprar</button>
        </div>
        <div class="produto">
            <img src="https://via.placeholder.com/150" alt="Produto 2">
            <h2>Produto 2</h2>
            <p>R$ 80,00</p>
            <button class="botao" onclick="adicionarAoCarrinho('Produto 2', 80)">Comprar</button>
        </div>
        <div class="produto">
            <img src="https://via.placeholder.com/150" alt="Produto 3">
            <h2>Produto 3</h2>
            <p>R$ 100,00</p>
            <button class="botao" onclick="adicionarAoCarrinho('Produto 3', 100)">Comprar</button>
        </div>
        <div class="produto">
            <img src="https://via.placeholder.com/150" alt="Produto 4">
            <h2>Produto 4</h2>
            <p>R$ 120,00</p>
            <button class="botao" onclick="adicionarAoCarrinho('Produto 4', 120)">Comprar</button>
        </div>
    </div>
    <h2>Carrinho</h2>
    <ul id="carrinho"></ul>
    <script>
        function adicionarAoCarrinho(nome, preco) {
            let item = document.createElement('li');
            item.textContent = `${nome} - R$ ${preco}`;
            document.getElementById('carrinho').appendChild(item);
        }
    </script>
</body>
</html>
