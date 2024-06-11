<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import Header from '../components/Header.vue'
</script>

<template>
    <Header />
  <main>
    <section class="techs">
      <div class="techs_title">
        <H1>My techs</H1> 
      </div>
      <div class="techs_show">
        <div class="front">
          <p>Fronted :</p>
          <div class="front_show">
            <img src="../assets/techs/html_icon.svg" alt="">
            <img src="../assets/techs/css_icon.svg" alt="">
            <img src="../assets/techs/bootstrap_icon.svg" alt="">
            <img src="../assets/techs/sass_icon.svg" alt="">
            <img src="../assets/techs/js_icon.svg" alt="">
            <img src="../assets/techs/ts_icon.svg" alt="">
            <img src="../assets/techs/vue_icon.svg" alt="">
            <img src="../assets/techs/react_icon.svg" alt="">
          </div>
        </div>
        <div class="back">
          <p>Backend :</p>
          <div class="front_show">
            <img src="../assets/techs/php_icon.svg" alt="">
            <img src="../assets/techs/mysql_icon.svg" alt="">
            <img src="../assets/techs/node_icon.svg" alt="">
            <img src="../assets/techs/express_icon.svg" alt="">
            <img src="../assets/techs/prisma_icon.svg" alt="">
            <img src="../assets/techs/python_icon.svg" alt="">
          </div>
        </div>
        <div class="cms">
          <p>CMS :</p>
          <div class="front_show">
            <img src="../assets/techs/wordpress_icon.svg" alt="">
          </div>
        </div>
        <div class="mobile">
          <p>Mobile :</p>
          <div class="front_show">
            <img src="../assets/techs/flutter_icon.svg" alt="">
          </div>
        </div>
        <div class="tools">
          <p>Tools :</p>
          <div class="front_show">
            <img src="../assets/techs/git_icon.svg" alt="">
            <img src="../assets/techs/postman_icon.png" alt="">
            <img src="../assets/techs/figma_icon.png" alt="">
            <img src="../assets/techs/blender_icon.svg" alt="">
          </div>
        </div>
      </div>
    </section>

    <section class="projects">
      <div class="projects_intro">
        <h1>Some of my projects</h1>
      </div>

      <div class="projects">
        <div class="project">
          <div class="top_part">
            <div class="project_title">
              Vue calling app
            </div>
            <div class="techs_used">
              <img src="../assets/techs/vue_icon.svg" alt="icone Vue.js">
            </div>
          </div>
          <div class="bottom_part">
            <div class="illustration">
              <img src="../assets/vue_calling_app.png" alt="screenchot vue calling app">
            </div>
            <div class="details">
              <ul>
                <li>
                  Calling contacts or numbers
                </li>
                <li>
                  Calls logs
                </li>
                <li>
                  Add contact function
                </li>
              </ul>
            </div>
          </div>
        </div>


        <div class="project">
          <div class="top_part">
            <div class="project_title">
              Pixel War
            </div>
            <div class="techs_used">
              <img src="../assets/techs/react_icon.svg" alt="React icon">
              <img src="../assets/techs/ts_icon.svg" alt="Typescript icon">
              <img src="../assets/techs/express_icon.svg" alt="Express icon">
              <img src="../assets/techs/prisma_icon.svg" alt="Prisma icon">
            </div>
          </div>
          <div class="bottom_part">
            <div class="illustration">
              <img src="../assets/pixel_war.png" alt="Screenshot Pixel war">
            </div>
            <div class="details">
              <ul>
                <li>
                  Canva to place pixels
                </li>
                <li>
                  Zoomable interface
                </li>
                <li>
                  Switching users autorisations
                </li>
              </ul>
            </div>
          </div>
        </div>



        <div class="project">
          <div class="top_part">
            <div class="project_title">
              Torcy's resource center
            </div>
            <div class="techs_used">
              <img src="../assets/techs/wordpress_icon.svg" alt="Wordpress icon">
            </div>
          </div>
          <div class="bottom_part">
            <div class="illustration">
              <img src="../assets/torcy.png" alt="Screenchot Torcy's website">
            </div>
            <div class="details">
              <ul>
                <li>
                  Adding new products
                </li>
                <li>
                  Granting permissions to users
                </li>
                <li>
                  Managing reserved products
                </li>
              </ul>
            </div>
          </div>
        </div>



        <div class="project">
          <div class="top_part">
            <div class="project_title">
              Micro blogging website
            </div>
            <div class="techs_used">
              <img src="../assets/techs/html_icon.svg" alt="html icon">
              <img src="../assets/techs/css_icon.svg" alt="css icon">
              <img src="../assets/techs/js_icon.svg" alt="javascript icon">
              <img src="../assets/techs/php_icon.svg" alt="php icon">
              <img src="../assets/techs/mysql_icon.svg" alt="mySQL icon">
              <img src="../assets/techs/python_icon.svg" alt="python icon">
            </div>
          </div>
          <div class="bottom_part">
            <div class="illustration">
              <img src="../assets/twitter.png" alt="Screenchot micro blogging website">
            </div>
            <div class="details">
              <ul>
                <li>
                  Stocking posts with user id
                </li>
                <li>
                  Filter system
                </li>
                <li>
                  automatically creating post with IOT
                </li>
              </ul>
            </div>
          </div>
        </div>



      </div>


    </section>
  </main>
</template>


<style lang="scss">
@import "node_modules/@glidejs/glide/src/assets/sass/glide.core";

main {
display: flex;
flex-direction: column;
align-items: center;

  section {
    height: 100vh;
    width: 70%;

    padding-top: 15vh;
    padding-bottom: 2.5%;

    .techs_title {
      display: flex;
      justify-content: center;
      align-items: center;

      h1{
        font-size: 2rem; 
      }
    }

    .techs_show{
      display: grid;
      grid-template-rows: repeat(5fr);

      div{
        
        p{
          font-size: 1.2rem;
        }

        div{

          margin-top: 1.2%;
          margin-bottom: 1.2%;
          display: flex;
          flex-wrap: wrap;
          gap: 5%;

          img{
            height: 7vh;
            transition: all 0.1s ease;
            filter: blur(2px);

            &:hover{
              transform: scale(1.5);
              transition: all 0.1s ease;
              filter: blur(0px);
              
            }
          }
        }
      }
    }

    .projects_intro{
      display: flex;
      justify-content: center;
      align-items: center;
      margin-bottom: 10%;

      h1{
        font-size: 2rem; 
      }
    }

    .projects{
      width: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      .project{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border: 3px solid #b94e56;
        padding: 5%;
        border-radius: 50px;
        margin-bottom: 10%;

        .top_part{
          display: flex;
          flex-wrap: wrap;
          justify-content: space-between;
          align-items: center;
          width: 100%;

          .project_title{

            font-size: 1.5rem;
            font-weight: bold;
          }
        }


        .bottom_part{
          display: flex;
          flex-wrap: wrap;
          justify-content: space-between;
          align-items: center;

          .illustration{
            width: 50%;

            img{
              width: 100%;
            }
          }

          .details{
            
            ul{

              li{
                padding-top: 5%;
                padding-bottom: 5%;
              }
            }
          }
        }
      }
    }
      
  }
}
</style>