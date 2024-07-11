<script setup>
import Header from '../components/Header.vue'
</script>

<template>
  <Header/>
  <main>
    <section id="introduction">
      <div class="pitch">
        <div class="picture">
          <img src="../assets/profile_picture.png" alt="profile picture">
        </div>
        <div class="informations">
          <h1>Quentin Garnier</h1>
          <p>Future full stack developer</p>
        </div>
      </div>
      <div class="next">
        <h2>Learn more about me</h2>
        <a href="#school">
          <img src="../assets/scroll_button.svg" alt="navigating button">
        </a>
      </div>
    </section>

    <section id="school">
      <div class="title">
        <div class="img">
          <img src="../assets/IIM_logo.png" alt="IIM logo">
        </div>
        <div class="context">
          <h1>IIM Digital School</h1>
          <h1>2nd year - Coding & Digital Innovation</h1>
        </div>
      </div>
      <div class="skills">
        <div class="card">
          <h2>Web developement</h2>
          <ul>
            <li>Frontend</li>
            <li>Backend</li>
            <li>IOT</li>
          </ul>
        </div>
        <div class="card">
          <h2>Project management</h2>
          <ul>
            <li>Understanding customer needs</li>
            <li>Tasks repartition</li>
            <li>Project monitoring</li>
          </ul>
        </div>
        <div class="card">
          <h2>Soft skills</h2>
          <ul>
            <li>Hackatons</li>
            <li>Design thinking</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="association">
      <div class="title">
        <div class="img">
          <img src="../assets/association_logo.png" alt="404 Devinci logo">
        </div>
        <div class="context">
          <h1>Association La 404 Devinci</h1>
          <h1>Project manager</h1>
        </div>
      </div>
      <div class="association_skills">
        <div class="asso_cards">
          <div class="asso_card">
            <h2>Association organisation</h2>
            <ul>
              <li>Projects imagination</li>
              <li>Developer</li>
            </ul>
          </div>
          <div class="asso_card">
            <h2>Community event</h2>
            <ul>
              <li>Team working</li>
              <li>Frontend & Backend experience</li>
              <li>Time constraint</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>



<style lang="scss">
main {

  display: flex;
  flex-direction: column;
  align-items: center;

  section {
    height: 100vh;
    width: 70%;

    padding-top: 7.5%;
    padding-bottom: 2.5%;

    .pitch{
      height: 65%;
      border: 3px solid #B94E56;
      border-radius: 50px;
      padding: 15px;
      background-color: #383852;
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-template-rows: 100%;
      align-items: center;
      justify-content: center;

      .picture{
        background-color: #383852;
        display: flex;
        align-items: center;
        justify-content: center;
        width: 65%;
        max-width: 225px;
        position: relative;
        margin-left: auto;
        margin-right: auto;

        img{          
          background-color: #383852;
          width: 100%;
        }

        &::after {
          content: '';
          position: absolute;
          left: 0%;
          bottom: 0px; /* Ajustement de la position */
          width: 100%;
          height: 5px;
          background-color: #B94E56;
          border-radius: 5px;
        }
      }

      .informations{
        display: grid;
        grid-template-rows: 1fr 1fr;  
        text-align: center;
        align-items: center;
        height: 50%;
        background-color: #383852;
      }

      h1{
        background-color: #383852;
        font-size: 2rem;
      }

      p{
        background-color: #383852;
        font-size: 1.2rem;
      }
    }

    .next{
      width: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 45%;

      bottom: 10%;
    }





    .title{
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 10%;
      height: 30%;
      margin-bottom: 10%;

      .img{

        display: flex;
        align-items: center;
        justify-content: center;

        img{
          width: 75%;
          object-fit: contain;
        }

      }

      .context{
        display: grid;
        grid-template-rows: 1fr 1fr;
        height: 100%;
        align-items: center;

        h1{
          font-size: 1.5rem;
        }
      }
      
    }

    .skills{
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 5%;
      

      .card{
        border: #B94E56 3px solid;
        border-radius: 10px;
        padding: 20px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10px;
        transition: all 0.2s ease;

        

        h2{
          font-size: 1.2rem;
          font-weight: bolder;
        }

        ul{
          
          li{
            font-size: 0.8rem;
          }
        }
      }

    }

    .association_skills{
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;

      .asso_cards{

        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 10%;
        width: 100%;

        .asso_card{
          border: #B94E56 3px solid;
          border-radius: 10px;
          padding: 20px;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
          gap: 10px;
          transition: all 0.2s ease;

          h2{
            font-size: 1.2rem;
            font-weight: bolder;
          }

          ul{
            
            li{
              font-size: 0.8rem;
            }
          }
        }

      }

    }

  }

  .card:hover{
    box-shadow: #B94E56 0px 5px 15px;
    transition: all 0.2s ease;
  }

  .asso_card:hover{
    transition: all 0.2s ease;
    transform: scale(1.2,1.2);
  }
}
</style>