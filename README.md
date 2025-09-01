<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Nom Prénom — Profil Chercheur</title>
  <meta name="description" content="Profil académique, publications, enseignement, projets et contact de Nom Prénom.">
  <link rel="canonical" href="https://votrePseudo.github.io/">
  <meta name="robots" content="index,follow">
  <meta name="theme-color" content="#0ea5e9">
  <!-- Open Graph -->
  <meta property="og:type" content="website">
  <meta property="og:title" content="Nom Prénom — Profil Chercheur">
  <meta property="og:description" content="Profil académique, publications, enseignement, projets et contact.">
  <meta property="og:url" content="https://votrePseudo.github.io/">
  
  <style>
    /* —— Design système léger, sans dépendances —— */
    :root{
      --bg: #0b0c0f; /* dark by default; JS peut forcer light */
      --fg: #e8eef7;
      --muted:#94a3b8;
      --card:#111318;
      --border:#1f2430;
      --accent:#0ea5e9; /* cyan-500 */
      --accent-2:#22c55e; /* green-500 */
      --warn:#f59e0b;
      --danger:#ef4444;
      --shadow: 0 10px 30px rgba(0,0,0,.35);
      --radius: 18px;
      --w: 1050px;
      --font: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji";
    }
    [data-theme="light"]{
      --bg:#f7fafc; --fg:#0b0c0f; --muted:#475569; --card:#ffffff; --border:#e5e7eb; --shadow:0 6px 24px rgba(2,6,23,.08);
    }
    html{scroll-behavior:smooth}
    body{margin:0; background:var(--bg); color:var(--fg); font-family:var(--font); line-height:1.6}
    a{color:var(--accent); text-decoration:none}
    a:hover{text-decoration:underline}
    .container{max-width:var(--w); margin-inline:auto; padding:24px}
    .skip{position:absolute; left:-999px}
    .skip:focus{left:12px; top:12px; background:var(--card); color:var(--fg); padding:8px 12px; border-radius:10px; outline:2px solid var(--accent)}
    header{position:sticky; top:0; backdrop-filter:saturate(180%) blur(8px); background:color-mix(in oklab, var(--bg), transparent 30%); border-bottom:1px solid var(--border); z-index:5}
    .nav{display:flex; align-items:center; gap:16px; justify-content:space-between; padding:12px 24px}
    .nav a.brand{font-weight:800; letter-spacing:.3px; color:var(--fg)}
    .nav .links{display:flex; gap:14px; flex-wrap:wrap}
    .btn{display:inline-flex; align-items:center; gap:8px; padding:10px 14px; border-radius:999px; border:1px solid var(--border); background:var(--card); color:var(--fg); box-shadow:var(--shadow)}
    .btn:hover{text-decoration:none; transform:translateY(-1px)}
    .btn.primary{background:linear-gradient(135deg, var(--accent), #38bdf8); color:white; border-color:transparent}
    .btn.ghost{background:transparent}
    .badge{display:inline-block; padding:6px 10px; border:1px solid var(--border); border-radius:999px; font-size:.85rem; color:var(--muted); background:color-mix(in oklab, var(--card), transparent 15%)}
    .hero{display:grid; grid-template-columns:1.2fr .8fr; gap:22px; padding:28px; background:radial-gradient(1200px 600px at 10% -20%, color-mix(in oklab, var(--accent), transparent 87%), transparent),
                         radial-gradient(1000px 600px at 100% 0%, color-mix(in oklab, var(--accent-2), transparent 90%), transparent)}
    .card{background:var(--card); border:1px solid var(--border); border-radius:var(--radius); padding:22px; box-shadow:var(--shadow)}
    h1{font-size:2.2rem; line-height:1.15; margin:0}
    h2{font-size:1.4rem; margin:0 0 10px}
    p{margin:10px 0}
    .muted{color:var(--muted)}
    .grid{display:grid; gap:18px}
    .grid.two{grid-template-columns:1fr 1fr}
    @media (max-width:920px){ .hero{grid-template-columns:1fr} .grid.two{grid-template-columns:1fr} }

    /* Sections */
    section{margin:28px 0}
    section header{position:static; background:none; border:none}
    .section-title{display:flex; align-items:center; justify-content:space-between; margin-bottom:10px}
    .list{display:grid; gap:14px}
    .pub{border:1px solid var(--border); border-radius:14px; padding:14px; background:color-mix(in oklab, var(--card), transparent 8%)}
    .pub .title{font-weight:700}
    .pub .meta{font-size:.95rem; color:var(--muted)}
    .pub .links{display:flex; gap:12px; flex-wrap:wrap; margin-top:8px}
    .chipset{display:flex; gap:8px; flex-wrap:wrap}
    .timeline{display:grid; gap:10px}
    .timeline .item{display:flex; gap:12px}
    .timeline .dot{width:10px; height:10px; border-radius:50%; background:var(--accent); margin-top:10px}

    footer{border-top:1px solid var(--border); padding:24px; color:var(--muted)}
    .icons{display:flex; gap:10px}
    .icon{width:22px; height:22px; display:inline-block; vertical-align:middle}
  </style>
</head>
<body>
  <a class="skip" href="#contenu">Aller au contenu</a>
  <header aria-label="Navigation principale">
    <nav class="nav container">
      <a class="brand" href="#">Nom&nbsp;Prénom</a>
      <div class="links" role="navigation" aria-label="Sections">
        <a href="#recherche">Recherche</a>
        <a href="#publications">Publications</a>
        <a href="#enseignement">Enseignement</a>
        <a href="#projets">Projets</a>
        <a href="#contact">Contact</a>
        <button id="themeToggle" class="btn ghost" type="button" aria-label="Changer de thème">🌓</button>
      </div>
    </nav>
  </header>

  <main id="contenu" class="container">
    <!-- —— HERO —— -->
    <section class="hero card" aria-labelledby="titre-hero">
      <div>
        <div class="chipset" aria-label="Mots-clés de recherche">
          <span class="badge">Hématologie</span>
          <span class="badge">Sécurité des données</span>
          <span class="badge">IA & Santé</span>
        </div>
        <h1 id="titre-hero">Nom Prénom</h1>
        <p class="muted"><strong>Titre actuel :</strong> Maître de conférences / Doctorant·e / Chercheur·se — <em>Institution / Laboratoire</em></p>
        <p>
          Courte bio (2–3 phrases). Présentez votre thématique, vos intérêts, et votre démarche scientifique. Exemple :
          « Je travaille sur la modélisation statistique des risques de brèches de données en santé et l'optimisation de tests d'hémostase. »
        </p>
        <div class="chipset" style="margin-top:12px">
          <a class="btn primary" href="mailto:votre.email@exemple.com">✉️ Me contacter</a>
          <a class="btn" href="CV.pdf" target="_blank" rel="noopener">📄 CV (PDF)</a>
          <a class="btn" href="https://scholar.google.com/" target="_blank" rel="noopener">🎓 Google Scholar</a>
          <a class="btn" href="https://orcid.org/0000-0000-0000-0000" target="_blank" rel="noopener">🧬 ORCID</a>
        </div>
      </div>
      <aside class="card" aria-label="Informations rapides">
        <h2>En bref</h2>
        <ul class="muted" style="padding-left:18px">
          <li>Domaines : hémostase, IA appliquée, cybersécurité</li>
          <li>Affiliation : <em>Université / CHU / Laboratoire</em></li>
          <li>Ville/Pays : …</li>
          <li>Disponibilité : collaborations, co‑encadrements, séminaires</li>
        </ul>
      </aside>
    </section>

    <!-- —— RECHERCHE —— -->
    <section id="recherche" aria-labelledby="titre-recherche">
      <div class="section-title">
        <h2 id="titre-recherche">Axes de recherche</h2>
        <span class="badge">màj facile</span>
      </div>
      <div class="grid two">
        <div class="card">
          <h3>Thème 1</h3>
          <p class="muted">Expliquez en 3–4 lignes la question scientifique, la méthode, et l'impact attendu.</p>
        </div>
        <div class="card">
          <h3>Thème 2</h3>
          <p class="muted">Idem, avec mots-clés et liens vers jeux de données ou dépôts de code si pertinents.</p>
        </div>
      </div>
    </section>

    <!-- —— PUBLICATIONS —— -->
    <section id="publications" aria-labelledby="titre-pubs">
      <div class="section-title">
        <h2 id="titre-pubs">Publications sélectionnées</h2>
        <a class="btn ghost" href="#toutes">Voir tout</a>
      </div>
      <div class="list">
        <!-- Copiez un bloc <article class="pub"> par publication -->
        <article class="pub">
          <div class="title">Titre de l'article de recherche</div>
          <div class="meta">Auteur·rice·s — <em>Revue/Conférence</em>, Année</div>
          <div class="links">
            <a href="#" class="badge" aria-label="Lien DOI">DOI</a>
            <a href="#" class="badge" aria-label="PDF">PDF</a>
            <a href="#" class="badge" aria-label="Code">Code</a>
          </div>
        </article>
        <article class="pub">
          <div class="title">Deuxième publication importante</div>
          <div class="meta">Auteur·rice·s — <em>Journal</em>, 2024</div>
          <div class="links">
            <a href="#" class="badge">DOI</a>
            <a href="#" class="badge">Résumé</a>
          </div>
        </article>
      </div>
      <details id="toutes" style="margin-top:10px">
        <summary class="btn ghost">Toutes les publications</summary>
        <div class="list" style="margin-top:10px">
          <article class="pub">
            <div class="title">Article complet (exemple)</div>
            <div class="meta">Nom, Nom — <em>Acta Medica</em>, 2023</div>
            <div class="links">
              <a href="#" class="badge">DOI</a>
              <a href="#" class="badge">PDF</a>
            </div>
          </article>
        </div>
      </details>
    </section>

    <!-- —— ENSEIGNEMENT —— -->
    <section id="enseignement" aria-labelledby="titre-teach">
      <h2 id="titre-teach">Enseignement</h2>
      <div class="timeline">
        <div class="item">
          <div class="dot" aria-hidden="true"></div>
          <div>
            <strong>Cybersecurity with Python</strong> — Master, 2024–
            <div class="muted">OWASP, PLS‑SEM, data leaks, ateliers pratiques</div>
          </div>
        </div>
        <div class="item">
          <div class="dot" aria-hidden="true"></div>
          <div>
            <strong>Hématologie clinique</strong> — 2023–
            <div class="muted">Hémostase, pathologies auto‑immunes, cas cliniques</div>
          </div>
        </div>
      </div>
    </section>

    <!-- —— PROJETS —— -->
    <section id="projets" aria-labelledby="titre-proj">
      <h2 id="titre-proj">Projets</h2>
      <div class="grid two">
        <div class="card">
          <h3>Projet A</h3>
          <p class="muted">Brève description du but, du rôle, et des résultats. Inclure un lien si open‑source.</p>
          <a class="btn" href="#">Dépôt GitHub</a>
        </div>
        <div class="card">
          <h3>Projet B</h3>
          <p class="muted">Description idem. Ajoutez un poster ou une démo si disponible.</p>
          <a class="btn" href="#">Site / Démo</a>
        </div>
      </div>
    </section>

    <!-- —— PRIX & BOURSES —— -->
    <section aria-labelledby="titre-awards">
      <h2 id="titre-awards">Distinctions</h2>
      <ul class="muted" style="padding-left:18px">
        <li>2025 — Lauréat·e Bourse XYZ</li>
        <li>2024 — Meilleure présentation, Conférence ABC</li>
      </ul>
    </section>

    <!-- —— CONTACT —— -->
    <section id="contact" aria-labelledby="titre-contact" class="card">
      <h2 id="titre-contact">Contact</h2>
      <p>📧 <a href="mailto:votre.email@exemple.com">votre.email@exemple.com</a></p>
      <p>🔗 Réseaux : 
        <a href="https://www.linkedin.com/" target="_blank" rel="noopener">LinkedIn</a> · 
        <a href="https://twitter.com/" target="_blank" rel="noopener">X/Twitter</a> · 
        <a href="https://www.researchgate.net/" target="_blank" rel="noopener">ResearchGate</a>
      </p>
    </section>
  </main>

  <footer class="container" role="contentinfo">
    <div class="icons" aria-label="Identifiants">
      <span class="badge">ORCID : 0000‑0000‑0000‑0000</span>
      <span class="badge">Scholar : /citations?user=XXXXX</span>
    </div>
    <p class="muted">© <span id="year"></span> Nom Prénom. Fichier unique prêt pour GitHub Pages.</p>
  </footer>

  <!-- Données structurées JSON‑LD (SEO) — à personnaliser -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Person",
    "name": "Nom Prénom",
    "jobTitle": "Titre/Grade",
    "affiliation": {"@type": "Organization", "name": "Université / CHU / Laboratoire"},
    "email": "votre.email@exemple.com",
    "url": "https://votrePseudo.github.io/",
    "sameAs": [
      "https://orcid.org/0000-0000-0000-0000",
      "https://scholar.google.com/citations?user=XXXXX",
      "https://www.linkedin.com/in/…"
    ],
    "knowsAbout": ["Hématologie", "Cybersécurité", "IA en santé"],
    "address": {"@type": "PostalAddress", "addressCountry": "MA"}
  }
  </script>

  <script>
    // —— Thème clair/sombre ——
    const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
    const saved = localStorage.getItem('theme');
    const root = document.documentElement;
    function applyTheme(mode){
      if(mode === 'light'){ root.setAttribute('data-theme','light'); }
      else { root.removeAttribute('data-theme'); }
      localStorage.setItem('theme', mode);
    }
    applyTheme(saved ? saved : (prefersDark ? 'dark' : 'light'));
    document.getElementById('themeToggle').addEventListener('click',()=>{
      const isLight = root.getAttribute('data-theme') === 'light';
      applyTheme(isLight ? 'dark' : 'light');
    });
    // Année automatique
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>

  <!-- Optionnel : analytics (collez votre script Plausible/GA ici) -->
</body>
</html>
