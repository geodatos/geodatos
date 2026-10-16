[index.html](https://github.com/user-attachments/files/33581227/index.html)
<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#102b3f">
  <meta name="description" content="GEODATOS brinda servicios técnicos digitales de topografía, ingeniería, movimiento de suelos, procesamiento de drones y documentación de obra.">
  <title>GEODATOS | Servicios técnicos digitales</title>
  <style>
    :root{--navy:#102b3f;--blue:#176b87;--cyan:#45c0c8;--ink:#172b3a;--muted:#5c6d79;--paper:#f4f7f8;--white:#fff;--line:#dce5e9}
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{margin:0;font-family:Inter,Segoe UI,Arial,sans-serif;color:var(--ink);line-height:1.65;background:#fff}
    a{color:inherit}
    .wrap{width:min(1120px,92%);margin:auto}
    header{background:rgba(16,43,63,.97);color:white;position:sticky;top:0;z-index:10;border-bottom:1px solid #ffffff20}
    .nav{min-height:76px;display:flex;align-items:center;justify-content:space-between;gap:20px}
    .brand{display:flex;align-items:center;gap:12px;text-decoration:none}
    .brand-logo{display:block;width:220px;max-width:45vw;height:auto;object-fit:contain}
    .brand strong{display:block;letter-spacing:2px;font-size:1.12rem;line-height:1.2}
    .brand small{display:block;font-size:.68rem;letter-spacing:1.5px;color:#c8d9e1;margin-top:4px}
    nav{display:flex;gap:22px;align-items:center}
    nav a{text-decoration:none;font-size:.9rem;color:#e0ebf0}
    nav a:hover{color:var(--cyan)}
    .nav-cta,.btn{display:inline-flex;align-items:center;justify-content:center;padding:12px 18px;border-radius:7px;text-decoration:none;font-weight:700;transition:.2s}
    .nav-cta,.btn-primary{background:var(--cyan);color:#09283a}
    .nav-cta:hover,.btn-primary:hover{background:#77d9dd;transform:translateY(-1px)}
    .hero{background:linear-gradient(120deg,#102b3f 0%,#164a64 64%,#176b87 100%);color:white;position:relative;overflow:hidden}
    .hero:before{content:"";position:absolute;inset:0;background-image:url('logo.png');background-repeat:no-repeat;background-position:78% 18%;background-size:min(68%,680px);opacity:.13;pointer-events:none;z-index:0}
    .hero:after{content:"";position:absolute;width:520px;height:520px;border:1px solid #ffffff18;border-radius:50%;right:-130px;top:-170px;box-shadow:0 0 0 55px #ffffff08,0 0 0 110px #ffffff05}
    .hero-grid{display:grid;grid-template-columns:1.2fr .8fr;gap:50px;align-items:center;padding:92px 0 100px;position:relative;z-index:1}
    @media(max-width:560px){.hero:before{background-size:95%;background-position:center 8%;opacity:.10}}
    .eyebrow{color:var(--cyan);font-size:.8rem;font-weight:800;letter-spacing:2px;text-transform:uppercase}
    h1{font-size:clamp(2.5rem,5vw,4.4rem);line-height:1.08;letter-spacing:-1.8px;margin:18px 0}
    .hero p{color:#d7e5eb;font-size:1.1rem;max-width:650px}
    .actions{display:flex;flex-wrap:wrap;gap:12px;margin-top:28px}
    .btn-outline{border:1px solid #ffffff70;color:#fff}
    .btn-outline:hover{background:#ffffff12}
    .hero-note{border:1px solid #ffffff2c;background:#ffffff0c;border-radius:16px;padding:28px;backdrop-filter:blur(3px)}
    .hero-note .big{font-size:3rem;font-weight:800;color:var(--cyan);line-height:1}
    .hero-note h3{margin:16px 0 8px;font-size:1.2rem}
    .hero-note p{font-size:.95rem;margin:0}
    .hero-tags{display:flex;gap:8px;flex-wrap:wrap;margin-top:25px}
    .tag{border:1px solid #ffffff30;padding:6px 10px;border-radius:999px;font-size:.78rem;color:#e5f0f4}
    section{padding:78px 0}
    .section-head{max-width:720px;margin-bottom:34px}
    .section-head h2{font-size:clamp(1.8rem,3vw,2.6rem);line-height:1.2;margin:10px 0 14px;letter-spacing:-.6px}
    .section-head p{color:var(--muted);margin:0}
    .services{background:var(--paper)}
    .service-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .service{background:white;border:1px solid var(--line);border-radius:12px;padding:25px;box-shadow:0 6px 20px #102b3f06}
    .service-num{width:38px;height:38px;border-radius:9px;background:#e0f6f6;color:#176b87;display:grid;place-items:center;font-weight:800;margin-bottom:18px}
    .service h3{font-size:1.08rem;line-height:1.35;margin:0 0 12px}
    .service ul{padding-left:18px;margin:0;color:var(--muted);font-size:.91rem}
    .service li{margin:7px 0}
    .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:55px;align-items:start}
    .about-grid h2{font-size:2.2rem;line-height:1.2;margin:10px 0 18px}
    .about-grid p{color:var(--muted)}
    .check-list{list-style:none;padding:0;margin:22px 0}
    .check-list li{padding:10px 0 10px 30px;position:relative;border-bottom:1px solid var(--line)}
    .check-list li:before{content:"✓";position:absolute;left:0;color:var(--blue);font-weight:900}
    .tools{background:var(--navy);color:white}
    .tools .section-head p{color:#c5d7df}
    .tool-grid{display:grid;grid-template-columns:repeat(5,1fr);gap:12px}
    .tool{padding:20px 12px;text-align:center;border:1px solid #ffffff25;border-radius:10px;background:#ffffff08}
    .tool strong{display:block;color:var(--cyan);font-size:1.05rem;margin-bottom:5px}
    .tool span{font-size:.82rem;color:#d4e1e7}
    .steps{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .step{padding:22px;border-left:3px solid var(--cyan);background:var(--paper);border-radius:0 10px 10px 0}
    .step b{display:block;margin-bottom:6px}
    .step p{font-size:.91rem;color:var(--muted);margin:0}
    .contact{background:#eaf4f6}
    .contact-box{display:grid;grid-template-columns:1.1fr .9fr;gap:40px;align-items:center;background:white;border-radius:16px;padding:clamp(24px,5vw,48px);border:1px solid var(--line)}
    .contact h2{font-size:2.3rem;line-height:1.2;margin:10px 0}
    .contact p{color:var(--muted)}
    .contact-links{display:grid;gap:12px}
    .contact-link{padding:15px 17px;border:1px solid var(--line);border-radius:9px;text-decoration:none;font-weight:700}
    .contact-link:hover{border-color:var(--blue);background:#f5fbfc}
    footer{background:#0a1e2b;color:#b9cbd4;padding:25px 0;font-size:.85rem}
    .footer-inner{display:flex;justify-content:space-between;gap:18px;flex-wrap:wrap}
    .small{font-size:.85rem;color:var(--muted)}
    @media(max-width:850px){nav{gap:12px}nav a:not(.nav-cta){display:none}.hero-grid,.about-grid,.contact-box{grid-template-columns:1fr}.hero-grid{padding:65px 0}.hero-note{max-width:500px}.service-grid{grid-template-columns:repeat(2,1fr)}.tool-grid{grid-template-columns:repeat(3,1fr)}}
    @media(max-width:560px){.service-grid,.steps{grid-template-columns:1fr}.tool-grid{grid-template-columns:repeat(2,1fr)}section{padding:58px 0}.brand-logo{width:190px}.hero-grid{gap:30px}}
  </style>
</head>
<body>
<header>
  <div class="wrap nav">
    <a class="brand" href="#inicio" aria-label="GEODATOS inicio">
      <img class="brand-logo" src="logo.png" alt="GEODATOS — Servicios técnicos digitales">
    </a>
    <nav aria-label="Navegación principal">
      <a href="#servicios">Servicios</a><a href="#nosotros">Cómo trabajamos</a><a href="#herramientas">Herramientas</a>
      <a class="nav-cta" href="#contacto">Solicitar presupuesto</a>
    </nav>
  </div>
</header>

<main>
  <section class="hero" id="inicio">
    <div class="wrap hero-grid">
      <div>
        <div class="eyebrow">Topografía · Ingeniería · Construcción</div>
        <h1>De los datos de campo a decisiones más claras.</h1>
        <p>Procesamiento topográfico, movimiento de suelos, planos y documentación técnica para acompañar tus proyectos de ingeniería y construcción.</p>
        <div class="actions">
          <a class="btn btn-primary" href="#contacto">Hablemos de tu proyecto ↗</a>
          <a class="btn btn-outline" href="#servicios">Ver servicios</a>
        </div>
        <div class="hero-tags"><span class="tag">Atención remota</span><span class="tag">Entregables digitales</span><span class="tag">Soporte técnico</span></div>
      </div>
      <aside class="hero-note">
        <div class="big">01—06</div>
        <h3>Soporte técnico para cada etapa</h3>
        <p>Desde el procesamiento de relevamientos y el control de obra hasta la documentación final conforme a obra.</p>
      </aside>
    </div>
  </section>

  <section class="services" id="servicios">
    <div class="wrap">
      <div class="section-head">
        <div class="eyebrow">Qué hacemos</div>
        <h2>Servicios técnicos digitales</h2>
        <p>Soluciones adaptadas al alcance, los datos disponibles y los requisitos de cada obra.</p>
      </div>
      <div class="service-grid">
        <article class="service"><div class="service-num">01</div><h3>Procesamiento de datos topográficos</h3><ul><li>Organización y revisión de datos de campo.</li><li>Superficies de terreno natural y proyecto.</li><li>Modelos digitales, perfiles y secciones.</li><li>Preparación de archivos para replanteos y controles.</li></ul></article>
        <article class="service"><div class="service-num">02</div><h3>Movimiento de suelos y control de obra</h3><ul><li>Cálculo de volúmenes de corte y terraplén.</li><li>Comparación entre relevamientos y proyecto.</li><li>Análisis de cotas, pendientes y geometrías.</li><li>Reportes de cantidades para revisión técnica.</li></ul></article>
        <article class="service"><div class="service-num">03</div><h3>Protocolos y documentación de calidad</h3><ul><li>Revisión y control documental.</li><li>Planillas, registros y reportes de seguimiento.</li><li>Verificación de información topográfica.</li><li>Identificación de inconsistencias y faltantes.</li></ul></article>
        <article class="service"><div class="service-num">04</div><h3>Planos conforme a obra (As-Built)</h3><ul><li>Actualización de planos con datos verificados.</li><li>Registro de modificaciones ejecutadas.</li><li>Actualización de cotas, dimensiones y pendientes.</li><li>Organización de archivos finales para revisión.</li></ul></article>
        <article class="service"><div class="service-num">05</div><h3>Relevamientos con drones</h3><ul><li>Procesamiento fotogramétrico de datos UAV.</li><li>Superficies, modelos digitales y nubes de puntos.</li><li>Ortomosaicos y curvas de nivel según los datos.</li><li>Volúmenes y comparación de superficies.</li></ul></article>
        <article class="service"><div class="service-num">06</div><h3>Diseño y modificación de planos</h3><ul><li>Dibujo y edición de planos técnicos 2D.</li><li>Modelos de terreno y documentación 3D.</li><li>Perfiles, secciones y detalles constructivos.</li><li>Conversión y organización de archivos CAD.</li></ul></article>
      </div>
    </div>
  </section>

  <section id="nosotros">
    <div class="wrap about-grid">
      <div>
        <div class="eyebrow">GEODATOS</div>
        <h2>Un soporte técnico que se integra a tu equipo.</h2>
        <p>Trabajamos junto a empresas constructoras, contratistas y profesionales para transformar información técnica en entregables claros, organizados y útiles para la planificación, ejecución y control de obra.</p>
        <p>La modalidad remota permite sumar capacidad de procesamiento sin ampliar la estructura operativa del cliente.</p>
      </div>
      <div>
        <h3>Cómo trabajamos</h3>
        <ul class="check-list">
          <li>Recepción de datos, planos y especificaciones.</li>
          <li>Revisión inicial y definición del alcance.</li>
          <li>Confirmación de formatos, plazos y entregables.</li>
          <li>Procesamiento, modelado, cálculo o documentación.</li>
          <li>Entrega digital y ajustes acordados.</li>
        </ul>
        <p class="small">Cada trabajo se cotiza según su complejidad, volumen de información, nivel de detalle y plazo de entrega.</p>
      </div>
    </div>
  </section>

  <section class="tools" id="herramientas">
    <div class="wrap">
      <div class="section-head">
        <div class="eyebrow">Entorno de trabajo</div>
        <h2>Herramientas digitales</h2>
        <p>Utilizamos software especializado de acuerdo con las necesidades y el alcance de cada proyecto.</p>
      </div>
      <div class="tool-grid">
        <div class="tool"><strong>Civil 3D</strong><span>Superficies, perfiles y volúmenes</span></div>
        <div class="tool"><strong>AutoCAD</strong><span>Dibujo y documentación técnica</span></div>
        <div class="tool"><strong>Pix4D</strong><span>Procesamiento fotogramétrico</span></div>
        <div class="tool"><strong>Revit</strong><span>Modelado BIM según alcance</span></div>
        <div class="tool"><strong>Formatos CAD</strong><span>DWG, DXF, PDF y compatibles</span></div>
      </div>
    </div>
  </section>

  <section>
    <div class="wrap">
      <div class="section-head">
        <div class="eyebrow">Proceso simple</div>
        <h2>De la consulta a la entrega</h2>
      </div>
      <div class="steps">
        <div class="step"><b>1. Nos contás el proyecto</b><p>Indicá el tipo de trabajo, la ubicación general y qué archivos tenés disponibles.</p></div>
        <div class="step"><b>2. Definimos el alcance</b><p>Revisamos la información y acordamos entregables, formato, plazo y presupuesto.</p></div>
        <div class="step"><b>3. Procesamos y entregamos</b><p>Desarrollamos el trabajo y entregamos los archivos digitales acordados.</p></div>
      </div>
    </div>
  </section>

  <section class="contact" id="contacto">
    <div class="wrap contact-box">
      <div>
        <div class="eyebrow">Contacto</div>
        <h2>¿Tenés un proyecto para cotizar?</h2>
        <p>Contanos qué necesitás y qué información tenés disponible. Te responderemos para revisar el alcance y preparar una propuesta.</p>
        <p class="small">Antes de publicar el sitio, reemplazá los datos de contacto de ejemplo por los tuyos.</p>
      </div>
      <div class="contact-links">
        <!-- WhatsApp GEODATOS: enlace en formato internacional, solo números. -->
        <a class="contact-link" href="https://wa.me/5493872118297" target="_blank" rel="noopener">↗ WhatsApp: +54 9 387 211-8297</a>
        <!-- Correo de contacto de GEODATOS. -->
        <a class="contact-link" href="mailto:geodatos.std@gmail.com?subject=Consulta%20de%20servicios%20GEODATOS">✉ geodatos.std@gmail.com</a>
        <a class="contact-link" href="mailto:geodatos.std@gmail.com?subject=Solicitud%20de%20presupuesto%20GEODATOS">＋ Solicitar presupuesto</a>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap footer-inner">
    <span><strong>GEODATOS</strong> — Servicios técnicos digitales</span>
    <span>Topografía · Ingeniería · Construcción</span>
    <span>© <span id="year">2026</span> GEODATOS</span>
  </div>
</footer>
</body>
</html>
