<template>

  <div class="menu">
    <link rel="shortcut icon" type="image/png" href="elo.png">
  <div class="image" :style="{ backgroundImage: 'url(' + background + ')' }">   
<div id="top">
<h1 id="h1" style="font-size:65px"> ZŁOTE USTA </h1> 
<h2 id="h2" style ="font-size:35px">KONKURS RECYTATORSKI NA WIŚNIOWEJ</h2> <br>
</div>
<div id="bottom">
<p style ="font-size:25px">BIBLIOTEKA SZKOLNA ZACHĘCA DO WZIĘCIA UDZIAŁU W IGRZYSKACH NA </p><br>
<p style ="font-size:25px">MIKROFONY, GDZIE ZWYCIĘZCA MOŻE BYĆ TYLKO JEDEN</p>
</div>
  </div>
<section class="questions-wrapper">
  <Question title="Gdzie i kiedy?" text="Konkurs odbędzie się w czytelni koło biblioteki
  w terminie podanym później." />
  <Question title="Kto organizuje?" text="Organizatorami konkursu są: Sylwia Błażejewska i Beata Walczak."/>
  <Question title="Kto może wziąć udział?" text="Konkurs jest ogólnoszkolny i każdy zainteresowany może w nim wystartować."/>
  <Question title="A będą jakieś nagrody?" text="Raczej nie."/>
  <Question title="Gdzie szukać więcej informacji?" text="Tu na stronie będą zamieszczane wszelkie niezbędne informacje dla zainteresowanych."/>
</section>

  </div>

  
</template>

<script>
import background from '@/assets/1.jpg';
import Question from '@/components/Question.vue'


export default {
  name: "Start",
  components: {
    Question
  },
  data() {
    return {
      background : background
    }
  }
}

</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');
html, body 
{

font-family: 'Lato', sans-serif;
}
#top
{
height: 40rem;
}
#bottom {
float: left;
}

.image {
  background-image: url({{background}});
  height: 50rem;
  display: flex;
  flex-direction: column;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
}

.questions-wrapper
{
  text-align: center;
  width: 100%;
  background-color: #36000C;
  padding: 3em;
  overflow: hidden;
}

.image,#h1 {
text-align: center;
color: gold;

}
.image,#h2 {
text-align: center;
color:white;

}




</style>