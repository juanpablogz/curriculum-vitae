<template>
  <div>
    <body>
      <header>
        <link
          rel="stylesheet"
          href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css"
          integrity="sha512-HK5fgLBL+xu6dm/Ii3z4xhlSUyZgTT9tuc/hSrtw6uzJOvgRr2a9jyxxT1ely+B+xFAmJKVSTbpM/CuL7qxO8w=="
          crossorigin="anonymous"
        />
        <nav id="navbar">
          <ul>
            <ul>
              <!-- <li><a href="#welcome-section">Juan Pablo Gómez</a></li>
            <li><a href="#welcome-section">Telefono</a></li>
            <li><a href="#welcome-section">+57 350 695 6606</a></li> -->
            </ul>
          </ul>
          <div class="portrait">
            <img
              src="https://res.cloudinary.com/dutj1bbos/image/upload/v1615503505/48387013_2163826213882758_4487837926322864128_n_pbain8.jpg"
              alt="dat_portrait"
            />
          </div>
          <ul>
            <li><a href="#welcome-section">Sobre mi</a></li>
            <li><a href="#experience">Experiencia</a></li>
            <li><a href="#skills">Habilidades</a></li>
            <li><a href="#projects">Proyectos</a></li>
          </ul>
        </nav>
      </header>
      <main>
        <section id="welcome-section">
          <h1>
            <div>Hola soy</div>
            <div>Juan Pablo <span class="highlight">Gómez zapata</span></div>
          </h1>
          <div class="info">
            Y constuyo cosas para la web
            <span class="highlight"></span>
          </div>
          <p>
            Soy programador de software, estudie en el sena (colombia) y en AIEP
            (chile) y me especializo en la creacion de sitios web, aplicaciones
            y todo lo que conlleva, mis tecnologias favoritas son Vuejs y ruby
            on rails.
          </p>
          <div class="contacts">
            <!-- <a href="https://codepen.io/quocdat1994" target="_blank">
              <i class="fab fa-codepen"></i>
            </a> -->
            <a
              id="profile-link"
              href="https://github.com/juanpablogz"
              target="_blank"
            >
              <i class="fab fa-github"></i>
            </a>
            <a href="https://www.linkedin.com/in/juan-pablo-b9a50a17b/" target="_blank">
              <i class="fab fa-linkedin"></i>
            </a>
            <a href="https://juanpablogz-d6d32.web.app/">
              <i class="fas fa-blog"></i>
            </a>
          </div>
        </section>
        <section id="experience">
          <h1 class="section-heading">Experiencia</h1>
          <div v-for="experience in experiences" :key="experience.id">
            <div class="experience">
              <h2>{{ experience.name }}</h2>
              <!-- <h3>Metanet</h3> -->
              <div>{{ experience.date }}</div>
              <p>
                {{ experience.description }}
              </p>
            </div>
          </div>
        </section>
        <section id="skills">
          <h1 class="section-heading">Habilidades</h1>
          <!-- <h2>Programming Languages</h2> -->
          <div class="icons">
            <i class="fab fa-html5" title="HTML"></i>
            <i class="fab fa-css3-alt" title="CSS"></i>
            <i class="fab fa-js" title="Javascript"></i>
            <i class="fab fa-vuejs" title="Vuejs"></i>
            <i class="fas fa-gem" title="ruby"></i>
            <i class="fab fa-bootstrap" title="Bootstrap"></i>
          </div>
          <div class="skills">
            <div>
              <h2>Software</h2>
              <ul>
                <li>Excel</li>
                <li>Word</li>
                <li>PowerPoint</li>
              </ul>
            </div>
            <div>
              <h2 style="padding: 0px 25px 0px 20px;">Lenguajes de programación</h2>
              <ul>
                <li>JavaScript. Conocimiento medio</li>
                <li>Ruby. Conocimiento básico</li>
              </ul>
            </div>
            <div>
              <h2>Framework</h2>
              <ul>
                <li>Vuejs. Conocimiento medio-alto</li>
                <li>Quasar. Conocimiento medio-alto</li>
                <li>Ruby On Rails. Conocimiento Basico</li>
                <li>Node + Express. Conocimiento Básico</li>
              </ul>
            </div>
            <div>
              <h2>estilos</h2>
              <ul>
                <li>CSS. Conocimiento medio-alto</li>
                <li>bootstrap. Conocimiento medio</li>
                <li>Tailwind. Conocimiento Básico</li>
              </ul>
            </div>
            <div>
              <h2>Bases de datos</h2>
              <ul>
                <li>PostgreSQL Conocimiento basico-medio</li>
                <li>MySql. Conocimiento básico-medio</li>
              </ul>
            </div>
            <div>
              <h2>Despligue</h2>
              <ul>
                <li>Netlify. Conocimiento medio</li>
                <li>Vercel. Conocimiento medio</li>
                <li>Heroku. Conocimiento Básico</li>
              </ul>
            </div>
          </div>
        </section>
        <section id="projects">
          <h1 class="section-heading">proyectos</h1>
          <div class="project-container">
            <div class="project-tile">
              <a href="https://www.since.love/">
                <img
                  src="https://res.cloudinary.com/dutj1bbos/image/upload/v1615506917/Captura_de_Pantalla_2021-03-11_a_la_s_6.55.05_p._m._bzdvya.png"
                  alt="project_1"
                  title="Project 1"
                />
              </a>
            </div>
            <div class="project-tile">
              <a href="https://estrellarestaurante.com/">
                <img
                  src="https://res.cloudinary.com/dutj1bbos/image/upload/v1615506999/Captura_de_Pantalla_2021-03-11_a_la_s_6.56.16_p._m._unupos.png"
                  alt="project_2"
                  title="Project 2"
                />
              </a>
            </div>
            <div class="project-tile">
              <a href="https://www.especialistaencasa.com/">
                <img
                  src="https://res.cloudinary.com/dutj1bbos/image/upload/v1615507060/Captura_de_Pantalla_2021-03-11_a_la_s_6.57.30_p._m._g4wm5i.png"
                  alt="project_3"
                  title="Project 3"
                />
              </a>
            </div>
            <div class="project-tile">
              <a href="https://exchange25.netlify.app/">
                <img
                  src="https://res.cloudinary.com/dutj1bbos/image/upload/v1615507108/Captura_de_Pantalla_2021-03-11_a_la_s_6.58.20_p._m._wmbyg7.png"
                  alt="project_4"
                  title="Project 4"
                />
              </a>
            </div>
            <!-- <div class="project-tile">
              <a href="#">
                <img
                  src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611334029/screenshot-zealous-mayer-c3bddc-netlify-app-1611334019534_rnakpp.png"
                  alt="project_5"
                  title="Project 5"
                />
              </a>
            </div> -->
          </div>
        </section>
      </main>
      <footer></footer>
    </body>
  </div>
</template>

<script>
export default {
  data() {
    return {
      experiences: [
        {
          name: "Especialista en casa",
          description:
            "Desarrollo front end de todo el software con el que se controlan servicios médicos, especialmente servicios de fisioterapia. Este servicio puede ser tomado de manera remota y en el domicilio del paciente",
          date: "Junio de 2018 - Presente (emprendimiento propio)"
        },
        {
          name: "31Rooms",
          description:
            "Desarrollador front end con vuejs, desarrollo de diversos proyectos con tecnologias como vuejs, nuxt y quasar. Proyectos como estrellarestaurante que es un listado de productos de un restaurante el cual puedes seleccionar segun preferencia y añadirle variantes, despues tienes las opciones de escoger el medio de pago y para finalizar el software te redirigue a whatsapp con un mensaje personalizado de tu pedido, sincelove que es un proyecto de citas en el cual me encargo del front end",
          date: "noviembre de 2020 - Presente"
        }
      ]
    };
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Saira+Extra+Condensed:wght@400&display=swap");

$primary-color: #54a0ff;

$primary-text-color: #6c757d;
$secondary-text-color: #343a40;

$primary-font: "Saira Extra Condensed", sans-serif;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  min-width: 320px;
  color: $primary-text-color;
  font-family: $primary-font;

  span.highlight {
    color: $primary-color;
  }
}

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $secondary-text-color;
  font-family: $primary-font;
}

// Header
header {
  width: 100%;
  padding: 1rem;
  background-color: $primary-color;
  position: sticky;
  top: 0;
  left: 0;
  z-index: 99;

  nav {
    .portrait {
      text-align: center;
      display: none;

      img {
        width: 100%;
        max-width: 160px;
        border-radius: 100%;
        border: 6px solid rgba(255, 255, 255, 0.3);
      }
    }

    ul {
      display: flex;
      justify-content: flex-end;
      list-style: none;

      li {
        margin-left: 1rem;

        a {
          color: white;
          font-size: 1.2rem;
          font-family: $primary-font;
          font-weight: bold;
          text-decoration: none;
          opacity: 0.5;
          letter-spacing: 1.5px;

          &:hover {
            opacity: 0.9;
          }
        }
      }
    }
  }
}

// Main
main {
  width: 100%;

  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    min-height: 65vh;
    padding: 0 1rem;
    border-bottom: 1px solid lighten($primary-text-color, 50);
    padding-top: 5rem;

    .section-heading {
      font-size: 4rem;
      color: $secondary-text-color;
      // text-transform: uppercase;
      margin-bottom: 3rem;
    }
  }

  section#welcome-section {
    h1 {
      div:first-child {
        font-size: 2.5rem;
        font-weight: 500;
        line-height: 0.5;
      }

      div:last-child {
        color: $secondary-text-color;
        font-size: 5.5rem;
      }
    }

    .info {
      font-weight: 600;
      font-size: 1.3rem;
      // text-transform: uppercase;
    }

    p {
      font-size: 1.3rem;
      margin: 2rem 0 1rem 0;
    }

    .contacts {
      a {
        width: 3rem;
        height: 3rem;

        display: inline-flex;
        justify-content: center;
        align-items: center;

        color: white;
        background-color: $secondary-text-color;
        font-size: 1.5rem;
        text-decoration: none;
        border-radius: 100%;
        margin-right: 0.5rem;

        &:hover {
          color: $primary-color;
        }
      }
    }
  }

  section#experience {
    padding-top: 5rem;
    .experience {
      margin-bottom: 2.5rem;

      h2 {
        font-size: 2rem;
        // text-transform: uppercase;
      }

      h3 {
        font-size: 1.5rem;
        color: $primary-text-color;
        // text-transform: uppercase;
      }

      div {
        color: $primary-color;
        font-size: 1.2rem;
        font-weight: 600;
        margin-bottom: 1rem;
      }

      p {
        font-size: 1.3rem;
      }
    }
  }

  section#skills {
    padding-top: 5rem;

    h2 {
      font-size: 2rem;
      color: $primary-text-color;
      text-transform: uppercase;
    }

    .icons {
      margin: 0.5rem 0 2rem 0;

      i {
        cursor: pointer;
        margin-right: 1rem;
        font-size: 3rem;

        &.fa-html5:hover {
          color: #e9633c;
        }

        &.fa-css3-alt:hover {
          color: #2862e9;
        }

        &.fa-js:hover {
          color: #f1d43b;
        }

        &.fa-react:hover {
          color: #49b7e8;
        }
        &.fa-bootstrap:hover {
          color: #533b78;
        }
        &.fa-sass:hover {
          color: #c85e93;
        }
      }
    }

    ul {
      list-style: square;

      li {
        font-size: 1.3rem;
        margin-left: 2rem;
      }
    }
  }
  .skills {
    display: flex;
    flex-wrap: wrap;
  }
  .bl {
  }
  section#projects {
    padding-top: 5rem;

    .project-container {
      width: 100%;
      display: grid;
      grid-template-columns: 1fr;
      grid-column-gap: 0.5rem;

      .project-tile {
        a {
          img {
            width: 100%;
            height: auto;

            filter: grayscale(100%);

            &:hover {
              filter: grayscale(0);
            }
          }
        }
      }
    }
  }
}

@media screen and (min-width: 480px) {
  main {
    section#projects {
      .project-container {
        grid-template-columns: repeat(2, 1fr);
      }
    }
  }
}

@media screen and (min-width: 568px) {
  main {
    section#experience {
      .experience {
        display: grid;
        grid-template-columns: auto auto;

        h2 {
          grid-column: 1 / span 2;
          grid-row: 1 / span 1;
          line-height: 1;
        }

        h3 {
          grid-column: 1 / span 2;
          margin-bottom: 0.5rem;
        }

        div {
          grid-column: 2 / span 1;
          grid-row: 1 / span 1;
        }

        p {
          grid-column: 1 / span 2;
        }
      }
    }
  }
}

@media screen and (min-width: 720px) {
  main {
    section#projects {
      .project-container {
        grid-template-columns: repeat(3, 1fr);
      }
    }
  }
}

@media screen and (min-width: 1024px) {
  body {
    display: grid;
    grid-template-columns: auto auto;
  }

  header {
    height: 100%;
    max-height: 100vh;

    nav {
      width: 15vw;
      max-width: 300px;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;

      .portrait {
        display: block;
      }

      ul {
        flex-direction: column;
        align-items: center;
        justify-content: center;

        li {
          margin: 0.6rem 0;

          a {
            font-size: 1.5rem;
          }
        }
      }
    }
  }

  main {
    section {
      padding: 0 3rem;
    }

    section#experience {
      .experience {
        display: grid;
        grid-template-columns: auto auto;

        h2 {
          grid-column: 1 / span 2;
          grid-row: 1 / span 1;
          line-height: 1;
        }

        h3 {
          grid-column: 1 / span 2;
          margin-bottom: 0.5rem;
        }

        div {
          grid-column: 2 / span 1;
          grid-row: 1 / span 1;
        }
      }
    }
  }
}

@media screen and (min-width: 1240px) {
  main {
    section#projects {
      .project-container {
        grid-template-columns: repeat(4, 1fr);
      }
    }
  }
}
</style>
