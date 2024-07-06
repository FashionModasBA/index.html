# index.html<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja de Camisetas e Shorts Estampados</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }
        header {
            background-color: #333;
            color: white;
            padding: 1rem;
            text-align: center;
        }
        main {
            padding: 2rem;
        }
        .product {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem;
            margin: 1rem 0;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }
        .product:hover {
            transform: scale(1.02);
        }
        .product img {
            max-width: 100px;
            border-radius: 8px;
        }
        .product-info {
            flex-grow: 1;
            padding: 0 1rem;
        }
        .product button {
            padding: 0.5rem 1rem;
            border: none;
            border-radius: 4px;
            background-color: #333;
            color: white;
            cursor: pointer;
            transition: background-color 0.3s ease-in-out;
        }
        .product button:hover {
            background-color: #555;
        }
        .sold-out {
            background-color: #888;
        }
    </style>
    <script>
        function toggleAvailability(button) {
            if (button.classList.contains('sold-out')) {
                button.classList.remove('sold-out');
                button.textContent = 'Disponível';
            } else {
                button.classList.add('sold-out');
                button.textContent = 'Esgotado';
            }
        }
    </script>
</head>
<body>
    <header>
        <h1>Loja de Camisetas e Shorts Estampados</h1>
    </header>
    <main>
        <div class="product">
            <img src="camiseta1.jpg" alt="Camiseta 1">
            <div class="product-info">
                <h2>Camiseta Estampada 1</h2>
                <p>Descrição da camiseta estampada 1.</p>
            </div>
            <button onclick="toggleAvailability(this)">Disponível</button>
        </div>
        <div class="product">
            <img src="camiseta2.jpg" alt="Camiseta 2">
            <div class="product-info">
                <h2>Camiseta Estampada 2</h2>
                <p>Descrição da camiseta estampada 2.</p>
            </div>
            <button onclick="toggleAvailability(this)">Disponível</button>
        </div>
        <div class="product">
            <img src="camiseta3.jpg" alt="Camiseta 3">
            <div class="product-info">
                <h2>Camiseta Estampada 3</h2>
                <p>Descrição da camiseta estampada 3.</p>
            </div>
            <button onclick="toggleAvailability(this)">Disponível</button>
        </div>
        <!-- Adicione mais produtos conforme necessário -->
    </main>
</body>
</html>
