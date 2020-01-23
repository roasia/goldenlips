<template>
  <div class="container">
    <div class="banner" v-bind:style="{ backgroundImage: 'url(' + image + ')' }">
      <div class="top">
        <div class="title">
          Złote usta
        </div>
        <div class="description">
          Konkurs krasomówczy na Wiśniowej
        </div>
      </div>
      <div class="bottom">
        <p>Biblioteka szkolna zachęca do wzięcia udziału w igrzyskach na mikrofony,</p> 
        <p>gdzie zwycięzca może być tylko jeden! </p>
      </div>
    </div>

    <div class="info">
      <div class="box">
        <question title="Gdzie i kiedy?" text="konkurs odbędzie się w czytelni koło biblioteki; termin konkursu zostanie podany póżniej"/>
        <question title="Kto organizuje?" text="organizatorami konkursu są: Sylwia Błażejewska oraz Beata Walczak"/>  
        <question title="Kto może wziąć udział?" text="W konkursie mogą wziać udział wszyscy uczniowie z naszej szkoły"/>  
        <question title="Czy będą jakieś nagrody?" text="zobaczymy"/>  
        <question title="Gdzie szukać więcej informacji?" text="Na tej stronie będą zamieszczane wszelkie niezbędne informacje dla zainteresowanych. Jeśli jednak wolisz bardziej werbalne środki przekazu, to panie z biblioteki mogą udzielić takich informacji"/>  


      </div>
    </div>

  </div>
</template>

<script>
import image from '@/assets/1.jpg';
import question from '@/components/Question';

export default {
  name: 'Start',
  components: {
    question
  },
  data() {
    return {
      image: image
    }
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');
  .container{
    width: 100vw;
    display: flex;
    flex-direction: column;
    font-family: 'Lato', sans-serif;
    color: rgba(255,255,255,0.5);

    .banner{
      width: 100vw;
      height: 100vh;
      display: flex;
      flex-direction: column;
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;

      .top{
        width: 100vw;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 20vh;

        .title{
          font-size: 5.5rem;
          color: #F4C621;
          text-transform: uppercase;
          padding-top: 5rem;
          font-weight: 900;
        }
        .description{
          font-size: 2rem;
          color: white;
          text-transform: uppercase;
          padding-top: 1.5rem;
        }
      }
      .bottom{
        width: 100vw;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: auto;
        font-size: 1.5rem;
        color: white;
        text-transform: uppercase;
        padding-bottom: 4rem;

        p{
          margin: 0;
          padding: 0.2rem;
        }
      }
    }
    .info{
      background-color: #36000C;
      min-height: 100vh;
      display: flex;
      justify-content: center;

      .box{
        width: 40vw;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding-bottom: 9vh;
      }
    }
  }

</style>