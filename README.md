<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Manual dos Padrinhos</title>
<style>
  /* Reset básico */
  body, html {
    margin: 0; padding: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #faf8fc;
    color: #4b3a5d;
    scroll-behavior: smooth;
  }

  header, footer {
    background: #e6def7;
    text-align: center;
    padding: 20px 10px;
    position: relative;
  }

  /* Lavandas topo e base */
  header::before, footer::after {
    content: "";
    display: block;
    background-image: url('https://i.imgur.com/R2y6oyF.png'); /* Lavanda decorativa */
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
    height: 80px;
  }
  header::before {
    margin-bottom: 10px;
  }
  footer::after {
    margin-top: 10px;
  }

  h1 {
    font-weight: 700;
    font-size: 2.5rem;
    margin-bottom: 10px;
    color: #6f4e7c;
  }

  nav {
    margin: 20px auto;
    text-align: center;
  }

  nav button {
    background: #9c88ff;
    border: none;
    color: white;
    padding: 10px 20px;
    margin: 0 10px;
    font-size: 1rem;
    border-radius: 25px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  nav button:hover {
    background: #7b66cc;
  }

  section {
    max-width: 700px;
    margin: 0 auto 40px;
    background: white;
    padding: 25px 30px;
    border-radius: 12px;
    box-shadow: 0 0 10px rgb(111 78 124 / 0.3);
  }

  section h2 {
    color: #6f4e7c;
    margin-bottom: 15px;
  }

  footer p {
    font-size: 0.9rem;
    color: #6f4e7c;
  }

  /* Esconder seções */
  .hidden {
    display: none;
  }

</style>
</head>
<body>

<header>
  <h1>Manual dos Padrinhos</h1>
</header>

<nav>
  <button onclick="showSection('intro')">Introdução</button>
  <button onclick="showSection('dicas')">Dicas</button>
  <button onclick="showSection('contato')">Contato</button>
</nav>

<main>
  <section id="intro">
    <h2>Sejam Bem-vindos!</h2>
    <p>Queridos padrinhos, é uma honra tê-los ao nosso lado nesse momento tão especial. Este manual foi feito para ajudar vocês a entenderem tudo sobre nosso grande dia e como podem contribuir para que seja inesquecível.</p>
  </section>

  <section id="dicas" class="hidden">
    <h2>Dicas Importantes</h2>
    <ul>
      <li>Cheguem com antecedência para os preparativos.</li>
      <li>Usem o traje indicado no convite.</li>
      <li>Estejam prontos para muitas fotos e diversão.</li>
      <li>Confirme presença e avisem sobre qualquer imprevisto.</li>
    </ul>
  </section>

  <section id="contato" class="hidden">
    <h2>Contato</h2>
    <p>Se precisar de algo, não hesite em nos chamar:</p>
    <ul>
      <li>Érika: (99) 99999-9999</li>
      <li>Pedro: (99) 98888-8888</li>
      <li>Email: casamento@erikaepedro.com</li>
    </ul>
  </section>
</main>

<footer>
  <p>© 2025 Érika & Pedro — Nosso grande dia com muito amor e lavanda 💜</p>
</footer>

<script>
  function showSection(id) {
    const sections = document.querySelectorAll('main section');
    sections.forEach(section => {
      section.classList.add('hidden');
    });
    document.getElementById(id).classList.remove('hidden');
  }
  // Mostrar a introdução por padrão
  showSection('intro');
</script>

</body>
</html>
