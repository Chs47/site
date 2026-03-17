[cite: 14, 15]
cd ~/Desktop/meus-projetos-git

[cite: 25, 26]
git clone https://github.com/seu-usuario/app-loja-roupas.git
cd app-loja-roupas

[cite: 90, 91]
git checkout -b feat/layout-dinamico

<div class="app-container">
  <header class="header">Moda & Estilo</header>
  <main class="main-content">
    <section class="product-grid">
      <article class="product-card">
        <img src="roupa1.jpg" alt="Camiseta">
        <h3>Camiseta Basic</h3>
        <p>R$ 89,90</p>
        <button class="btn-comprar">Comprar</button>
      </article>
    </section>
  </main>
  <footer class="footer">© 2026 TechBuild Solutions</footer>
</div>

/* Layout Principal com Grid */
.app-container {
  display: grid;
  grid-template-areas: "header" "main" "footer";
  grid-template-rows: 80px 1fr 60px;
  height: 100vh;
}

/* Alinhamento de Itens com Flexbox */
.product-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 1px solid #ddd;
  transition: transform 0.3s; /* Animação suave */
}

.product-card:hover {
  transform: scale(1.05); /* Efeito dinâmico */
}

