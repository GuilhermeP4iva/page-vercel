# page-vercel<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Paiva Digital</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: radial-gradient(circle at top, #1e293b, #020617);
      color: #fff;
    }

    header {
      display: flex;
      justify-content: space-between;
      padding: 20px 40px;
      align-items: center;
    }

    header h2 {
      margin: 0;
    }

    .btn {
      background: linear-gradient(135deg, #3b82f6, #22c55e);
      padding: 12px 25px;
      border-radius: 10px;
      border: none;
      cursor: pointer;
      color: white;
      font-weight: bold;
    }

    .hero {
      text-align: center;
      padding: 100px 20px;
    }

    .hero h1 {
      font-size: 48px;
      margin-bottom: 20px;
    }

    .hero p {
      color: #94a3b8;
      max-width: 600px;
      margin: auto;
      margin-bottom: 30px;
    }

    .glass {
      backdrop-filter: blur(10px);
      background: rgba(255,255,255,0.05);
      border-radius: 15px;
      padding: 20px;
      margin: 20px;
    }

    .features {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 60px 20px;
    }

    .feature {
      width: 260px;
      margin: 10px;
    }

    .form {
      text-align: center;
      padding: 60px 20px;
    }

    .form-box {
      max-width: 400px;
      margin: auto;
    }

    input {
      width: 100%;
      padding: 12px;
      margin-bottom: 12px;
      border-radius: 8px;
      border: none;
    }

    footer {
      text-align: center;
      padding: 20px;
      color: #64748b;
    }
  </style>
</head>

<body>

<header>
  <h2>🚀 Paiva Digital</h2>
  <button class="btn" onclick="scrollForm()">Contato</button>
</header>

<section class="hero">
  <h1>Sua empresa no próximo nível</h1>
  <p>Soluções digitais inteligentes para aumentar faturamento e produtividade</p>
  <button class="btn" onclick="scrollForm()">Começar agora</button>
</section>

<section class="features">
  <div class="feature glass">
    <h3>💡 Inovação</h3>
    <p>Tecnologias modernas para seu negócio</p>
  </div>

  <div class="feature glass">
    <h3>⚙️ Automação</h3>
    <p>Reduza custos e aumente eficiência</p>
  </div>

  <div class="feature glass">
    <h3>📈 Crescimento</h3>
    <p>Escale seu negócio com segurança</p>
  </div>
</section>

<section class="form" id="form">
  <h2>Solicite uma proposta</h2>

  <div class="form-box">
    <form onsubmit="sendLead(event)">
      <input type="text" placeholder="Nome" required>
      <input type="email" placeholder="Email" required>
      <button class="btn">Enviar</button>
    </form>
  </div>
</section>

<footer>
  © 2026 Paiva Digital
</footer>

<script>
  function scrollForm() {
    document.getElementById("form").scrollIntoView({ behavior: "smooth" });
  }

  function sendLead(e) {
    e.preventDefault();
    alert("Lead enviado 🚀");
  }
</script>

</body>
</html>
