<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Belleza divina</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #fff5f8;
      padding: 20px;
    }

    header {
      text-align: center;
      padding: 20px 0;
      background-color: #ffccda;
      margin-bottom: 20px;
    }

    header h1 {
      color: #5c2a4a;
    }

    .share-button {
      text-align: center;
      margin-bottom: 30px;
    }

    .share-button button {
      background-color: #cc3366;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 8px;
      cursor: pointer;
    }

    .share-button p {
      color: green;
      display: none;
      margin-top: 10px;
    }

    .seccion {
      margin-bottom: 40px;
    }

    .seccion h2 {
      margin-bottom: 20px;
      color: #cc3366;
      text-align: center;
    }

    .cards-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 20px;
      justify-content: center;
    }

    .card {
      background-color: white;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 20px;
      transition: transform 0.3s;
      text-align: center;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card img {
      max-width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 15px;
    }

    .card h3 {
      margin-bottom: 10px;
      color: #d6336c;
    }

    .card p {
      color: #555;
    }
  </style>
</head>
<body>
  <header>
    <h1>Belleza divina</h1>
  </header>

  <div class="share-button">
    <button onclick="compartirPagina()">Compartir esta página</button>
    <p id="mensaje-copiado">¡Enlace copiado al portapapeles!</p>
  </div>

  <script>
    function compartirPagina() {
      const url = window.location.href;
      navigator.clipboard.writeText(url).then(() => {
        const mensaje = document.getElementById("mensaje-copiado");
        mensaje.style.display = "block";
        setTimeout(() => {
          mensaje.style.display = "none";
        }, 2000);
      });
    }
  </script>

  <section class="seccion">
    <h2>Maquillaje</h2>
    <div class="cards-container">
      <div class="card">
        <img src="https://locatelcolombia.vtexassets.com/arquivos/ids/214672/7509552828429_1-BASE-LIQUIDA-VOGUE-RESIST-FPS-15-X-30--ML.jpg?v=636984705372300000" alt="Base Líquida">
        <h3>Base Líquida</h3>
        <p><strong>Precio: $30,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://ame.com.co/cdn/shop/products/POLVO-MX-TONO-01.jpg?v=1696267929" alt="Polvo Compacto">
        <h3>Polvo Compacto</h3>
        <p><strong>Precio: $23,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_778183-MCO82920897315_032025-E.webp" alt="Paleta de Sombras">
        <h3>Paleta de Sombras</h3>
        <p><strong>Precio: $70,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://samycosmetics.vtexassets.com/arquivos/ids/156290/025114-1.jpg?v=637757985206170000" alt="Labial Mate">
        <h3>Labial Mate</h3>
        <p><strong>Precio: $15,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTqYVldofMwXZ8WJbtmQczhaExR8DgO8q4Htw&s" alt="Rubor Líquido">
        <h3>Rubor Líquido</h3>
        <p><strong>Precio: $21,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQyT2lhW9sAai5jyVNrKJltpv7LAy-NKquWSg&s" alt="Rubor Compacto">
        <h3>Rubor Compacto</h3>
        <p><strong>Precio: $18,000 COP</strong></p>
      </div>
    </div>
  </section>

  <section class="seccion">
    <h2>Cuidado del Cabello</h2>
    <div class="cards-container">
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_608296-MLU75604530794_042024-E.webp" alt="Mascarilla">
        <h3>Mascarilla</h3>
        <p><strong>Precio: $28,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://images.rappi.com/products/42f1fd42-7513-40e0-88c2-e099e22405bd.png?e=webp&q=80&d=130x130" alt="Shampoo">
        <h3>Shampoo</h3>
        <p><strong>Precio: $24,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_749520-MCO43061351415_082020-E.webp" alt="Aceite para el Cabello">
        <h3>Aceite capilar</h3>
        <p><strong>Precio: $35,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_771515-MLU72972319955_112023-E.webp" alt="Cepillo Alisador">
        <h3>Cepillo Alisador</h3>
        <p><strong>Precio: $75,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_949182-MLU75612164104_042024-E.webp" alt="Termoprotector">
        <h3>Termoprotector</h3>
        <p><strong>Precio: $29,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_NQ_NP_654789-MLU75021628304_032024-O.webp" alt="Tratamiento Rizos">
        <h3>Tratamiento de Rizos</h3>
        <p><strong>Precio: $38,000 COP</strong></p>
      </div>
    </div>
  </section>

  <section class="seccion">
    <h2>Cuidado Facial</h2>
    <div class="cards-container">
      <div class="card">
        <img src="https://http2.mlstatic.com/D_NQ_NP_775255-MLU73656643277_122023-O.webp" alt="Shampoo Facial">
        <h3>Jabon Facial</h3>
        <p><strong>Precio: $20,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_992281-MLU78592526244_082024-E.webp" alt="Serum">
        <h3>Serum</h3>
        <p><strong>Precio: $45,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_775996-MLU74724538538_032024-E.webp" alt="Mascarilla">
        <h3>Mascarilla</h3>
        <p><strong>Precio: $22,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_989788-MLA74220129619_012024-E.webp" alt="Desmaquillante">
        <h3>Desmaquillante</h3>
        <p><strong>Precio: $18,000 COP</strong></p>
      </div>
    </div>
  </section>

  <section class="seccion">
    <h2>Fragancias y Accesorios</h2>
    <div class="cards-container">
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_879053-MLA82953610445_032025-E.webp" alt="Perfume">
        <h3>Perfume</h3>
        <p><strong>Precio: $60,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_Q_NP_2X_832992-MCO43496892396_092020-E.webp" alt="Set de Brochas">
        <h3>Set de Brochas</h3>
        <p><strong>Precio: $50,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_NQ_NP_600901-MLA74192178885_012024-O.webp" alt="Crema de Chocolate">
        <h3>Crema de Chocolate</h3>
        <p><strong>Precio: $26,000 COP</strong></p>
      </div>
      <div class="card">
        <img src="https://http2.mlstatic.com/D_NQ_NP_975814-CBT81549194482_012025-O.webp" alt="Espejo con Luz">
        <h3>Espejo con Luz</h3>
        <p><strong>Precio: $40,000 COP</strong></p>
      </div>
    </div>
  </section>
</body>
</html>
