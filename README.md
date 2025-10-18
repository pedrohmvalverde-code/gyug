<!--
  Arquivo: site-simples.html
  Instruções: Salve este arquivo como site-simples.html e abra no navegador.
  Este é um template responsivo de página única (hero, serviços, portfólio, contato).
  Posso personalizar textos, cores, imagens, integrar com formulário real, gerar React/Tailwind, 
  ou empacotar como zip para deploy. Diga o que quer mudar!
-->

<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Meu Site — Seu Nome/Marca</title>
  <meta name="description" content="Website simples e responsivo criado rapidamente">
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --accent:#06b6d4;
      --muted:#94a3b8;
      --glass: rgba(255,255,255,0.04);
      --radius:14px;
      --maxw:1100px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;background:linear-gradient(180deg,var(--bg),#071025);color:#e6eef6;line-height:1.5}
    .container{max-width:var(--maxw);margin:0 auto;padding:32px}
    header{display:flex;justify-content:space-between;align-items:center;padding:12px 0}
    .logo{font-weight:700;letter-spacing:0.2px}
    nav{display:flex;gap:18px}
    a{color:inherit;text-decoration:none}
    .btn{background:var(--accent);color:#022; padding:10px 14px;border-radius:10px;font-weight:600}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:32px;align-items:center;padding:48px 0}
    .card{background:var(--card);padding:28px;border-radius:var(--radius);box-shadow:0 6px 30px rgba(2,6,23,0.6)}
    h1{font-size:32px;margin:0 0 12px}
    p.lead{color:var(--muted);margin:0 0 20px}
    .cta-row{display:flex;gap:12px}

    /* Features / Services */
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:28px}
    .feature{background:var(--glass);padding:16px;border-radius:12px}
    .feature h3{margin:8px 0 6px;font-size:16px}
    .feature p{margin:0;color:var(--muted);font-size:14px}

    /* Portfolio */
    .portfolio-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:18px}
    .thumb{height:140px;background-size:cover;background-position:center;border-radius:10px}

    /* Contact */
    form{display:grid;gap:10px}
    input,textarea{background:#071226;border:1px solid rgba(255,255,255,0.04);padding:12px;border-radius:8px;color:inherit}
    textarea{min-height:120px}

    footer{color:var(--muted);padding:30px 0;text-align:center}

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr;}
      .grid-3{grid-template-columns:1fr}
      .portfolio-grid{grid-template-columns:repeat(2,1fr)}
      header{gap:12px}
    }
    @media (max-width:520px){
      .portfolio-grid{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">SuaMarca</div>
      <nav>
        <a href="#servicos">Serviços</a>
        <a href="#portfolio">Portfólio</a>
        <a href="#contato" class="btn">Contato</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div>
          <div class="card">
            <h1>Crio sites bonitos e rápidos para você.</h1>
            <p class="lead">Design responsivo, performance otimizada e experiência pensada para converter visitantes em clientes. Posso construir seu site completo ou um protótipo rápido.</p>
            <div class="cta-row">
              <a href="#contato" class="btn">Solicitar orçamento</a>
              <a href="#portfolio">Ver portfólio</a>
            </div>
            <div class="grid-3" style="margin-top:20px">
              <div class="feature">
                <strong>Landing pages</strong>
                <p>Foco em conversão e velocidade.</p>
              </div>
              <div class="feature">
                <strong>Sites institucionais</strong>
                <p>Apresente sua empresa com profissionalismo.</p>
              </div>
              <div class="feature">
                <strong>Loja online</strong>
                <p>Integração com pagamentos e gestão simples.</p>
              </div>
            </div>
          </div>
        </div>

        <aside>
          <div class="card">
            <h3>Resumo rápido</h3>
            <p style="color:var(--muted)">Tempo estimado: 1–2 semanas (dependendo do escopo). Preço: varia conforme funcionalidades.</p>
            <hr style="opacity:0.06;margin:12px 0">
            <h4>O que entrego</h4>
            <ul style="color:var(--muted);padding-left:18px">
              <li>HTML/CSS/JS ou React</li>
              <li>Design responsivo</li>
              <li>Treinamento básico para editar</li>
            </ul>
            <div style="margin-top:12px"><a href="#contato" class="btn">Vamos conversar</a></div>
          </div>
        </aside>
      </section>

      <section id="portfolio" style="margin-top:28px">
        <h2>Portfólio</h2>
        <p style="color:var(--muted)">Alguns exemplos rápidos (imagens de placeholder).</p>
        <div class="portfolio-grid">
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1519389950473-47ba0277781c?auto=format&fit=crop&w=800&q=60')"></div>
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1521737604893-d14cc237f11d?auto=format&fit=crop&w=800&q=60')"></div>
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=800&q=60')"></div>
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1508385082359-f9b0b6b8d0b3?auto=format&fit=crop&w=800&q=60')"></div>
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1531497865149-6fb1d6a1f0d8?auto=format&fit=crop&w=800&q=60')"></div>
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1509395176047-4a66953fd231?auto=format&fit=crop&w=800&q=60')"></div>
        </div>
      </section>

      <section id="servicos" style="margin-top:28px">
        <h2>Serviços</h2>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-top:12px">
          <div class="card">
            <h3>Criação de site</h3>
            <p style="color:var(--muted)">Site completo com design personalizado, SEO básico e largura responsiva.</p>
          </div>
          <div class="card">
            <h3>Manutenção</h3>
            <p style="color:var(--muted)">Atualizações, backups e pequenas mudanças mensais.</p>
          </div>
        </div>
      </section>

      <section id="contato" style="margin-top:28px">
        <h2>Contato</h2>
        <div class="card" style="margin-top:12px">
          <form action="mailto:seuemail@exemplo.com" method="post" enctype="text/plain">
            <input type="text" name="nome" placeholder="Seu nome" required>
            <input type="email" name="email" placeholder="Seu e‑mail" required>
            <input type="text" name="assunto" placeholder="Assunto">
            <textarea name="mensagem" placeholder="Como posso ajudar?" required></textarea>
            <div style="display:flex;gap:10px;justify-content:flex-end">
              <button type="submit" class="btn">Enviar</button>
              <button type="reset" style="background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px;border-radius:8px;color:var(--muted)">Limpar</button>
            </div>
          </form>
        </div>
      </section>

    </main>

    <footer>
      <div style="max-width:var(--maxw);margin:18px auto 0;padding:0 32px">© <span id="year"></span> SuaMarca — Feito com ❤️</div>
    </footer>
  </div>

  <script>
    // Atualiza ano no rodapé
    document.getElementById('year').innerText = new Date().getFullYear();
  </script>
</body>
</html>
