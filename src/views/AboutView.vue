<script setup>
import Header from '../components/Header.vue'
</script>

<template>
  <Header/>

  <main class="main">
    <div class="contact_part">
      <div class="contact_speach">
        <h1>Currently looking for an apprenticeship</h1>
        <p>Feel free to contact me</p>
      </div>
      <div class="contact_inputs">
        <a href="mailto:quentingarnier92320@gmail.com" target="_blank"><img src="../assets/mail_logo.png" alt="Icone de mail"></a>
        <a href="https://www.linkedin.com/in/quentin-garnier-07a58824b/" target="_blank"><img src="../assets/linkedin_logo.png" alt=""></a>
      </div>
    </div>

    <div class="cv_part">
      <div class="cv">
        <img src="../assets/CV_Alternance_Quentin_Garnier.png" alt="CV">
      </div>
    </div>
  </main>
</template>

<style lang="scss">
  .main{

    display: grid;
    grid-template-columns: 1fr 1fr;

    justify-content: center;
    align-items: center;

    width: 100%;
    height: 100vh;

    

    .contact_part{
      display: grid;
      grid-template-rows: 1fr 1fr;

      .contact_speach{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 10%;

        h1{
          text-decoration: underline;
          font-size: 1.5rem;
        }
      }

      .contact_inputs{

        display: flex;
        justify-content: space-around;
        align-items: center;
        a{

          width: 30%;
          img{

            width: 100%;
          }
        }
      }
    }

    .cv_part{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      .cv{
        width: 50%;

        img{
          width: 100%;
        }
      }
    }
  }
</style>