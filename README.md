<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Confeitaria Delícia</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #fff8f5;
    }

    header {
      background: #ffb6b9;
      padding: 20px;
      text-align: center;
      color: white;
    }

    h1 {
      margin: 0;
    }

    .banner {
      background: url('https://images.unsplash.com/photo-1578985545062-69928b1d9587') center/cover;
      height: 300px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-size: 30px;
      font-weight: bold;
    }

    .container {
      padding: 20px;
    }

    .produtos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .produto {
      background: white;
      border-radius: 10px;
      padding: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }

    .produto img {
      width: 100%;
      border-radius: 10px;
    }

    .btn {
      background: #ff6f61;
      color: white;
      padding: 10px;
      border: none;
      cursor: pointer;
      border-radius: 5px;
      margin-top: 10px;
    }

    form {
      display: grid;
      gap: 10px;
      max-width: 500px;
      margin: auto;
    }

    input, textarea {
      padding: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }

    /* WhatsApp botão */
    .whatsapp {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25d366;
      color: white;
      padding: 15px;
      border-radius: 50%;
      font-size: 20px;
      text-decoration: none;
    }

    .pagamentos {
      text-align: center;
      margin-top: 20px;
    }
  </style>
</head>

<body>

<header>
  <h1>Confeitaria Delícia</h1>
  <p>Bolos artesanais feitos com amor</p>
</header>

<div class="banner">
  Encomende seu bolo perfeito 🎂
</div>

<div class="container">

  <h2>🍰 Nossos Bolos</h2>

  <div class="produtos">
    
    <div class="produto">
      <img src="https://images.unsplash.com/photo-1605470375648-278bcbd579a6">
      <h3>Bolo de Chocolate</h3>
      <p>R$ 80,00</p>
      <button class="btn">Selecionar</button>
    </div>

    <div class="produto">
      <img src="https://images.unsplash.com/photo-1621303837174-89787a7d4729">
      <h3>Bolo de Morango</h3>
      <p>R$ 90,00</p>
      <button class="btn">Selecionar</button>
    </div>

    <div class="produto">
      <img src="https://images.unsplash.com/photo-1588195538326-c5b1e9f80a1b">
      <h3>Bolo Personalizado</h3>
      <p>A partir de R$ 120,00</p>
      <button class="btn">Selecionar</button>
    </div>

  </div>

  <h2>📝 Fazer Pedido</h2>

  <form id="pedidoForm">
    <input type="text" placeholder="Nome completo" required>
    <input type="tel" placeholder="WhatsApp" required>
    <input type="email" placeholder="Email" required>

    <input type="text" placeholder="Rua" required>
    <input type="text" placeholder="Número" required>
    <input type="text" placeholder="Bairro" required>
    <input type="text" placeholder="Cidade" required>
    <input type="text" placeholder="CEP" required>

    <input type="date" required>
    <textarea placeholder="Detalhes do pedido"></textarea>

    <button class="btn" type="submit">Enviar Pedido</button>
  </form>

  <div class="pagamentos">
    <h2>💳 Formas de Pagamento</h2>
    <p>✔ PIX | ✔ Cartão | ✔ Boleto</p>
  </div>

</div>

<footer>
  <p>© 2026 Confeitaria Delícia</p>
  <p>Contato: (27) 99999-9999</p>
</footer>

<!-- Botão WhatsApp -->
<a class="whatsapp" href="https://wa.me/5527999999999" target="_blank">
  💬
</a>

<script>
  document.getElementById("pedidoForm").addEventListener("submit", function(e){
    e.preventDefault();
    alert("Pedido enviado com sucesso! Entraremos em contato pelo WhatsApp.");
  });
</script>

</body>
</html>
