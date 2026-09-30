<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="DESTINA S.A.S. — La brújula para tu futuro profesional. Orientación académica, becas y oportunidades laborales.">
<title>DESTINA S.A.S. | La brújula para tu futuro profesional</title>
<style>
:root {
  --blue:#1677d2;
  --blue-dark:#0755a2;
  --yellow:#ffd83d;
  --yellow-soft:#fff4b8;
  --sky:#eaf6ff;
  --ink:#15304b;
  --muted:#5e7286;
  --white:#ffffff;
  --line:#d9e8f4;
  --shadow:0 18px 45px rgba(12,70,120,.12);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{
  font-family:Inter,Segoe UI,Arial,sans-serif;
  color:var(--ink);
  background:linear-gradient(180deg,#f8fcff 0%,#eef8ff 55%,#fffdf2 100%);
  line-height:1.6;
}
a{color:inherit;text-decoration:none}
.container{width:min(1120px,92%);margin:auto}
header{
  position:sticky;top:0;z-index:50;
  background:rgba(255,255,255,.94);
  backdrop-filter:blur(12px);
  border-bottom:1px solid var(--line);
}
.nav{
  min-height:76px;display:flex;align-items:center;justify-content:space-between;gap:20px;
}
.brand{display:flex;align-items:center;gap:12px;font-weight:900;color:var(--blue-dark)}
.brand img{width:52px;height:52px;object-fit:contain;border-radius:50%}
.brand span{font-size:1.15rem;letter-spacing:.5px}
nav{display:flex;gap:8px;flex-wrap:wrap}
nav a{padding:9px 13px;border-radius:999px;font-weight:700;color:#36566f;font-size:.93rem}
nav a:hover{background:var(--yellow-soft);color:var(--blue-dark)}

.hero{padding:82px 0 62px;overflow:hidden}
.hero-grid{display:grid;grid-template-columns:1.15fr .85fr;gap:50px;align-items:center}
.badge{display:inline-flex;align-items:center;gap:8px;background:var(--yellow-soft);border:1px solid #f0d45a;color:#705900;padding:8px 14px;border-radius:999px;font-weight:800;font-size:.86rem}
h1{font-size:clamp(2.6rem,6vw,5rem);line-height:.98;margin:18px 0 16px;letter-spacing:-2px}
h1 .accent{color:var(--blue)}
.lema{font-size:clamp(1.15rem,2vw,1.45rem);font-weight:800;color:var(--blue-dark);margin-bottom:18px}
.hero p{font-size:1.05rem;color:var(--muted);max-width:680px}
.actions{display:flex;gap:12px;flex-wrap:wrap;margin-top:28px}
.btn{display:inline-flex;align-items:center;justify-content:center;padding:13px 20px;border-radius:14px;font-weight:900;border:2px solid transparent;transition:.2s}
.btn-primary{background:var(--blue);color:white;box-shadow:0 10px 24px rgba(22,119,210,.22)}
.btn-primary:hover{transform:translateY(-2px);background:var(--blue-dark)}
.btn-secondary{background:white;border-color:var(--blue);color:var(--blue-dark)}
.btn-secondary:hover{background:var(--sky)}
.hero-card{position:relative}
.compass{width:min(360px,82vw);aspect-ratio:1;margin:auto;border-radius:50%;background:white;border:13px solid var(--yellow);box-shadow:0 0 0 8px var(--blue),var(--shadow);display:grid;place-items:center;position:relative}
.compass::before{content:"";width:72%;height:72%;border:4px solid var(--blue);border-radius:50%;position:absolute}
.compass img{width:42%;height:42%;object-fit:contain;position:relative;z-index:2;border-radius:50%}
.compass .n{position:absolute;top:9%;font-weight:900;color:var(--blue-dark)}
.compass .e{position:absolute;right:9%;font-weight:900;color:var(--blue-dark)}
.compass .s{position:absolute;bottom:9%;font-weight:900;color:var(--blue-dark)}
.compass .w{position:absolute;left:9%;font-weight:900;color:var(--blue-dark)}

section{padding:72px 0}
.section-title{text-align:center;max-width:760px;margin:0 auto 38px}
.section-title h2{font-size:clamp(2rem,4vw,3rem);margin-bottom:10px}
.section-title p{color:var(--muted)}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:20px}
.card{background:rgba(255,255,255,.9);border:1px solid var(--line);border-radius:22px;padding:26px;box-shadow:var(--shadow)}
.icon{width:48px;height:48px;border-radius:15px;display:grid;place-items:center;background:var(--yellow);font-size:1.35rem;margin-bottom:15px}
.card h3{margin-bottom:8px;font-size:1.18rem}
.card p{color:var(--muted);font-size:.96rem}

.about{background:linear-gradient(135deg,#0d67b9,#1590dc);color:white}
.about .section-title p,.about .card p{color:#e7f5ff}
.about .card{background:rgba(255,255,255,.1);border-color:rgba(255,255,255,.2);box-shadow:none}
.about .icon{color:var(--ink)}

.feature-list{display:grid;grid-template-columns:repeat(2,1fr);gap:16px}
.feature{display:flex;gap:14px;padding:18px;background:white;border:1px solid var(--line);border-radius:18px;box-shadow:0 8px 25px rgba(12,70,120,.07)}
.check{flex:0 0 30px;width:30px;height:30px;border-radius:50%;display:grid;place-items:center;background:var(--yellow);font-weight:900;color:#4c4200}

.qr-section{background:linear-gradient(135deg,#fff7bd,#ffffff)}
.qr-wrap{display:grid;grid-template-columns:1fr 340px;gap:35px;align-items:center;background:white;border:1px solid #f0dc78;border-radius:28px;padding:35px;box-shadow:var(--shadow)}
.qr{width:250px;max-width:100%;display:block;margin:auto;border-radius:12px}
.note{margin-top:14px;color:#8a7200;font-size:.86rem;background:#fff9d9;padding:10px 12px;border-radius:12px}

.socials{display:flex;gap:12px;flex-wrap:wrap;margin-top:18px}
.social{background:white;border:1px solid var(--line);padding:12px 15px;border-radius:14px;font-weight:800;color:var(--blue-dark)}
.social:hover{border-color:var(--blue);background:var(--sky)}

footer{background:#082f55;color:#dcefff;padding:35px 0}
.footer-grid{display:flex;justify-content:space-between;gap:25px;flex-wrap:wrap}
footer strong{color:white}
.small{font-size:.88rem;color:#a9c8df;margin-top:8px}

@media(max-width:850px){
  .hero-grid,.qr-wrap{grid-template-columns:1fr}
  .hero{padding-top:55px}
  .grid-3{grid-template-columns:1fr}
  .feature-list{grid-template-columns:1fr}
  nav{display:none}
  .qr-wrap{text-align:center}
}
</style>
</head>
<body>

<header>
  <div class="container nav">
    <a class="brand" href="#inicio">
      <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/4gHYSUNDX1BST0ZJTEUAAQEAAAHIAAAAAAQwAABtbnRyUkdCIFhZWiAH4AABAAEAAAAAAABhY3NwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQAA9tYAAQAAAADTLQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAlkZXNjAAAA8AAAACRyWFlaAAABFAAAABRnWFlaAAABKAAAABRiWFlaAAABPAAAABR3dHB0AAABUAAAABRyVFJDAAABZAAAAChnVFJDAAABZAAAAChiVFJDAAABZAAAAChjcHJ0AAABjAAAADxtbHVjAAAAAAAAAAEAAAAMZW5VUwAAAAgAAAAcAHMAUgBHAEJYWVogAAAAAAAAb6IAADj1AAADkFhZWiAAAAAAAABimQAAt4UAABjaWFlaIAAAAAAAACSgAAAPhAAAts9YWVogAAAAAAAA9tYAAQAAAADTLXBhcmEAAAAAAAQAAAACZmYAAPKnAAANWQAAE9AAAApbAAAAAAAAAABtbHVjAAAAAAAAAAEAAAAMZW5VUwAAACAAAAAcAEcAbwBvAGcAbABlACAASQBuAGMALgAgADIAMAAxADb/2wBDAAYEBQYFBAYGBQYHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQcHBwoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCABkAGQDASIAAhEBAxEB/8QAHAABAAIDAQEBAAAAAAAAAAAAAAUHBAYIAwIB/8QAOhAAAQMEAAMFBQYDCQAAAAAAAQIDBAAFBhEHIUESEzFRYRQyQnGBFSJSU2KhIzNyCBYkJTSCkbHB/8QAGgEBAAIDAQAAAAAAAAAAAAAAAAIEAwUGAf/EAC8RAAEDAgUBBgUFAAAAAAAAAAEAAgMEEQUSITFBURNhgZGh4RQyccHRBjNi8PH/2gAMAwEAAhEDEQA/AOn6UpREpSlESvN95qOyt19xDTSBtS1qCUpHmSa9K584m3pV7yK7Nz4qLhAt0+PZ7Za3VkMSJziQsuvge8Eg8geWgeprFNKIm5iL/kr1oubK87berXdFrRbblClrR7yWH0uEfMA1IVzhe8OuFguloavDFgiyp61NW+62CIYT0KSEFSUqA99s6I5/Xxq4uFeSvZZglsusxCUTVJUzJCfDvW1FCiPQlO9dN1CKfO8xubZwsfA/4vS2wuFttKUqwopSlKIlKUoiUpSiJSlQ+WZJa8Usb92vklMeGzyJ8SpR8EpHVR6CiKYrnri3AtthymY5c5zbdkv8hh4vNSEIfts5vkl4JJ5oIA2enPfKszJb/fL7bXrllt2cwvFSR3UNhYTNkJPh3rnigkfAkE+daSrJcesrcc4rgCZgkPIYTPuukrcWs6B7TgW4Qf8AaK1U9U2qDoadjpCNy3YEfyNhcLIAIrOkcG368+CzchypDku2Pu5rByu8IWpi2MN9xFYjOrSUl53SjvQJ5nQHQbNXzwxx9jF8ItdpjykS1MtlTr6FbDjqiVLUPTtE69NVz09xAlG4Q4FxwKxTfbFKQ2004gk6Gz7zevAVKWReOPXptvF510wPJF80RVjTD6vLuiS2sb6JI+W6xs+Jw4ufXRPBO7jYgDgHLsNenKCWKos2F4PcPddNUqs8M4hTBemcazyKzbr69v2SSySY08D8sn3V+aT5/SrMrbRyMlaHsNweVAgg2KUpSprxKUpREpSlEX4pQSkqUQEgbJPSud7pkkS/z7hxBv5Wcbsri49jia2H3EnsqkaPIqKvup8vpVl8dby/ZOF95dhKKZcpCYTKh4hTqgjY9QCSKpjiI7b7ZkeHYhJlx4NotUUSXO9UEoUtOkI3vxO+0r12aoVuaZ8dGw5TIbE9GjU/jxUs4iY6Yi+UbdTws7G8en5XchkeXbdkLO40Q824ifwpHh2vNXjvwrcL/jUC8Wd22SUqbbJS4h2OrsLbWk7SoHoRUjblQpEFh+A+h2OpALa21BSSB5EV7y3kRYyn5DyG2GwVqccUAEjzPpXXwwQ08IghaAwcLjpJpZZe1kN3LQbBwvt9ovUa6PXW4z1xyS0JLoUEkjRI0PLlWxZDbLDkCVWi4pjOyFo71Lfa/jISOXbHUc+taTfeI32q1NZxWQxGgxz2Xrkv72z1DLfio/qVpI9eVY3A60B6XcMnle0rdmHstOvrK3C2PBRPmdbPgPDQ1Uw4v+UXBvr/AHfgLI+NzRnkNiLWHPtyVMNQ1ylr4f5fKdkh5syLJdyNO7Rz7JP5iNg76jxq0ODmVTL3aZtov3LIbG77JMP5w1tDw/qT+4NVhxgu9siWUuN3OHHv9tcbnw2lODthaDvWvHShsa67qbt10TA4xYneIg7EPKLcqK+noVJSHGyfUe78ia4uenbhuICOL9uW+nRw1PmF1FFO6rpsz/mb6hXtSlK2KmlKUoiUpSiKrf7RJCcLtji/5Ld6hKc/p70bqoeLN4bsfFqU9ILiS9bWktlDRcOg4vteAPXVX9xgx5zJ+HF7tsYbllnvo/q62QtI+pTr61SmW3FmbBw7iLH05FQ2ItyQRsoSsgK7Q/Q4kg/PdUzMKbEaad1rXLddRdw0v5KM7DJTSMbva+mh0UlwMLzOCsiSFtpL7ykNrBBCVOFQ+703vevWte4xXdc+4RrK00qTboC2p12ZaOitrtjTXqSNq16D0qzLtc4tmx6TdgE+yx2VP/wtaI1sa11O6ojG7VkGXl2S8l2BHnvGTJeA288T4BI+FAGgCfnXSVrZHsEEAuT6Dr3LSYZ8P2zqmsdZgudNyTsApDPXsVzS72SBgUZph0dpM56LFMdKI+vcUOyNnloCrrsMRu2WliK02EBCQkdnlrlrXyHhUJiGIQLBHbZjtNthJ5pHPtHzUfFR9a2pAClK5ghGteeq9w3D24dTinDy/m5N1Trq01s3aZco4H3KobPrs3ZL7lMea0+25Nc7wL9nKw417O2kff14AhY9OdbkwFpPBZpX+pD7B9dBjn/5WbxRP2nHhYpDKftK9PBkK1vuWAQXXD5ADfz3UnY4bd+44WyPDH+W4nAKl65gOuDsIR8+zz+lc9jcgkraamba7S5x62sd/E6LoMIBMEkrubDytsr0pSlWFZSlKURKUpREqhMptjHDvIbg1coqXeH2ROKU6pY2iBJXyUlXk2vz6H5c77rFudviXSA/BuMZqTEfSUOMup7SVg9CKr1VMyqiMUmx9OhHeFJjyx2YLnZh6Zw8R7FeO9uGGqH+DuaE977Og+Db4Hw+S+fT5CRyG/R7TjEafjC4ktc2Q3FYcLnba7S1a2ojmQPKpSdgmVYN3ysIcbv2PKJ3ZJ7mnGUnoy4eRH6VfvVe3trh6+s/3ox+9YfcFLClFLbjCSodQU7bPPrrdYoMYrqBnY1TC8cPbqfEb381UmwmnqJBLGbHkH7LOsud31vKLTbbuqC9GnFbQUw2pCmylJUDzJB8NdK2zIM0gwJotkFt2739aSlq3xD21lWvjI5IHUk+A51WjULhFGkNPv5JerqtBPYZVJWTs8tDu0JVz8ORrdcfcvUlv2Hhfgos8R3kq53Jox0Afi0duL+uzVqf9RmW7aCB5J2zaAfUn3WGPAwCHVDx325WO669haHLteO7uvEG9JEaHCj/AHu5B91lsfhHIqV1P/JtvhFhi8Qxtf2isPX24uGXcXt726r4R+lI5D6nrWNw74ZxMZmOXm7zHL1kz405PfH8sfhaT8Kf3/6qwqp0dI+Nzp53ZpH7nj6DuHqtm9zcojjFmhKUpV9Y0pSlESlKURKUpREr5WlK0lK0hST4gjYNfVKIsdiFFjr7UeMw0o9UNhJ/asilKIlKUoiUpSiJSlKIlKUoiUpSiJSlKIlKUoiUpSiJSlKIlKUoi//Z" alt="Logotipo original de DESTINA">
      <span>DESTINA S.A.S.</span>
    </a>
    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#nosotros">Nosotros</a>
      <a href="#servicios">Servicios</a>
      <a href="#oportunidades">Oportunidades</a>
      <a href="#descargar">Aplicación</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </div>
</header>

<main>
<section class="hero" id="inicio">
  <div class="container hero-grid">
    <div>
      <span class="badge">✦ Orientación académica y laboral</span>
      <h1>Tu futuro tiene <span class="accent">rumbo.</span></h1>
      <div class="lema">“La brújula para tu futuro profesional”</div>
      <p>
        DESTINA S.A.S. es una aplicación digital integral que organiza información sobre
        carreras, becas y oportunidades laborales para acompañar a jóvenes, egresados y
        personas que buscan nuevas rutas académicas o profesionales.
      </p>
      <div class="actions">
        <a class="btn btn-primary" href="#descargar">Conoce la aplicación</a>
        <a class="btn btn-secondary" href="#servicios">Ver servicios</a>
      </div>
    </div>
    <div class="hero-card">
      <div class="compass" aria-label="Brújula inspirada en el logotipo de DESTINA">
        <span class="n">N</span><span class="e">E</span><span class="s">S</span><span class="w">O</span>
        <img src="data:image/jpeg;base64,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" alt="Logo DESTINA">
      </div>
    </div>
  </div>
</section>

<section id="nosotros" class="about">
  <div class="container">
    <div class="section-title">
      <h2>¿Qué es DESTINA?</h2>
      <p>
        Una herramienta tecnológica pensada para centralizar información y facilitar la
        construcción del proyecto de vida académico y profesional.
      </p>
    </div>
    <div class="grid-3">
      <article class="card"><div class="icon">🧭</div><h3>Orientación</h3><p>Apoya la exploración de intereses, habilidades y rutas de formación para tomar decisiones informadas.</p></article>
      <article class="card"><div class="icon">🎓</div><h3>Formación</h3><p>Reúne información sobre carreras, instituciones, becas y alternativas educativas.</p></article>
      <article class="card"><div class="icon">💼</div><h3>Empleabilidad</h3><p>Facilita el acceso a oportunidades laborales, prácticas y pasantías mediante información organizada.</p></article>
    </div>
  </div>
</section>

<section id="servicios">
  <div class="container">
    <div class="section-title">
      <h2>Lo que encontrarás</h2>
      <p>Contenido organizado para acompañar diferentes momentos de tu camino académico y profesional.</p>
    </div>
    <div class="feature-list">
      <div class="feature"><div class="check">✓</div><div><h3>Oportunidades académicas</h3><p>Explora alternativas de formación y rutas educativas según tus necesidades.</p></div></div>
      <div class="feature"><div class="check">✓</div><div><h3>Becas y convocatorias</h3><p>Consulta información sobre beneficios y oportunidades de acceso a la educación.</p></div></div>
      <div class="feature"><div class="check">✓</div><div><h3>Oportunidades laborales</h3><p>Encuentra información sobre empleos, prácticas y experiencias preprofesionales.</p></div></div>
      <div class="feature"><div class="check">✓</div><div><h3>Información centralizada</h3><p>Reduce la dispersión de información y facilita la búsqueda desde un solo entorno digital.</p></div></div>
      <div class="feature"><div class="check">✓</div><div><h3>Perfil y recomendaciones</h3><p>La propuesta contempla información y sugerencias relacionadas con el perfil del usuario.</p></div></div>
      <div class="feature"><div class="check">✓</div><div><h3>Conexión con fuentes oficiales</h3><p>DESTINA orienta al usuario hacia las fuentes de terceros donde se realizan las postulaciones.</p></div></div>
    </div>
  </div>
</section>

<section id="oportunidades" class="qr-section">
  <div class="container">
    <div class="qr-wrap">
      <div>
        <span class="badge">📱 DESTINA S.A.S.</span>
        <h2 style="font-size:2.4rem;margin:14px 0 10px">Lleva tu brújula contigo</h2>
        <p style="color:var(--muted)">
          La propuesta de DESTINA está pensada como una aplicación móvil accesible desde
          dispositivos digitales, con información académica y laboral organizada.
        </p>
        <div class="socials">
          <a class="social" href="https://www.instagram.com/destina.oficial_f.a.m/" target="_blank" rel="noopener">Instagram</a>
          <a class="social" href="https://www.facebook.com/" target="_blank" rel="noopener">Facebook: Destina Destina</a>
          <a class="social" href="https://www.tiktok.com/@Destina_oficial" target="_blank" rel="noopener">TikTok</a>
          <a class="social" href="https://www.youtube.com/" target="_blank" rel="noopener">YouTube: Destina.oficial_f.a.m</a>
        </div>
      </div>
      <div id="descargar">
        <img class="qr" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAeoAAAHqAQAAAADjFjCXAAAEDklEQVR4nO2dXYrjOhBGT10b8mjDLKCX4uyglzRrujuwl5IFDMiPAzI1D/pz0nO5EHvoafLVQ4iJDsJQVKm+khRzDtjyzxEahAsXLly4cOHChZ+LW7Yes3EzWC192JXNdkOuaxl6PW924S+KT+7uHoDpdnGWEcze3Fmsx65rD1PoHOjc3d3v8YOzC38xnORDUyD5lc9DhMkjTAF8pnOfARgi7sX1kp/OX/rdhX8W3j88G1ycZQwOaxeBzXzyrWea+aiyfOl3F/634DnNBmAZN2Nyd7MxP9r1z84u/LXwwWsi/ZmKBhgisPZpreczkD7c48mzC39JfDEzsxHsul7Sys2+3y5u1zKwPG6phD11duEvhqd13d2CbTNf3iK+jB0OP81Zgfx4v7b70u8u/LPwXQ2bc+jgqUBNv+bHCAzud2Wualjhz1qS35IiMhRf89BlNSXpJW0InacFn7xO+POWY53HpM3tohnUuFZ9sgl5Lq8T/rRl9wF8LnGN1IIIOeo15TjrKu5SiYUfsbKu63zXjEi+VrpfRS8pvubyOuHHzKsl0W5XXKTHuz4YxSfldcIPWItcpP5qqGJwCXhpYGrVFu+U1wk/YLsdJFkgifu2GKXCKMk1D5HXCT9gzeva/pJcV4QyZKaoKTshRV4n/Gm7qxLKGq4m0lK0NtGuLfjkdcKftX2GDVWvIwt0qTdRf82SXnVCeZ3wp6zEusiDLFeCW6lcU/4dvLqevE74s5aD1tCaYXkh9xj6phoTd9iXfnfhn4U/qr9JL8kRjl33K2+3A5RhhZ+pEtfWfl3StbbYTj6ZUawTfshyrAtdFuPyuZ2iEu+L1ljbsqphhR+yVk1ArVyTVNe+AR+SsLxO+FF8vXjRhrdyZIL6bXDPp3XWnnRa9nrm7MJfC681bNzl1dJzjdzJdzX/ujpiwg9Zy5u78iHtW2/ffL95ve3Dk9cJf8rSaR2DLhoYMDiw9pFl7CKshi/jjzxuCng6qH3K7MJfE6+xruwlofS82ibPfKBil4RRhhV+xIpycn9GpzUj6rUndQuUlBPhp2RYB8dKrIss7wFfrItM/17cWL85yzvpVwMrx2K/9LsL/yy8nta577kGSMFtHh52sAO600n4MXxfw+a2GDQhpfVcaVlXyonwY/h+f13tw5biIvdcc78sUE/GSjkRfgKe2l0BmG49sPa438olOssILG/7QvbU2YW/GP77uzqBeiXsw7aU8oMyrPCn7eNdnUPn5Z6wzXx5DxjDj578EYB1M9Wwwk/Ep7BZ3lo8ROx7SriXstPkZsbyFrHrH5ld+Evgd3uJ250m7aBYa1V4682qmhB+yB5r2FqlUgW6duNJEVLkdcKPmPn/j/lv07/XCRcuXLhw4cKF/y34L6hrksRfv4BDAAAAAElFTkSuQmCC" alt="Código QR de DESTINA">
        <div class="note"><strong>Importante:</strong> este QR es provisional porque no se proporcionó el enlace oficial de descarga de la aplicación. Al tenerlo, se puede reemplazar por un QR que abra directamente la app.</div>
      </div>
    </div>
  </div>
</section>

<section id="contacto">
  <div class="container">
    <div class="section-title">
      <h2>DESTINA S.A.S.</h2>
      <p>La brújula para tu futuro profesional</p>
    </div>
    <div class="grid-3">
      <article class="card"><div class="icon">📸</div><h3>Instagram</h3><p>@destina.oficial_f.a.m</p></article>
      <article class="card"><div class="icon">f</div><h3>Facebook</h3><p>Destina Destina</p></article>
      <article class="card"><div class="icon">▶</div><h3>YouTube</h3><p>Destina.oficial_f.a.m</p></article>
    </div>
    <div class="card" style="margin-top:20px;text-align:center">
      <h3>TikTok</h3><p>@Destina_oficial</p>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="container footer-grid">
    <div>
      <strong>DESTINA S.A.S.</strong>
      <div class="small">La brújula para tu futuro profesional</div>
    </div>
    <div class="small">Orientación · Educación · Oportunidades</div>
  </div>
</footer>

</body>
</html>
