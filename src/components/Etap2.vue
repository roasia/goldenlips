<template>
  <div class="container">
    <div class="title">
      Chcę wziąć udział
    </div>
    <div class="main">
      <div class="left">
        <div class="single-name">
          Imię
        </div>
        <div class="single-name">
          Nazwisko
        </div>
        <div class="single-name">
          Klasa
        </div>
        <div class="single-name">
          Temat
        </div>
         <div class="single-name">
          email
        </div>
        </div>
      <div class="right">
        <div class="single-input"><input type="text" v-model="imie" ></div>
        <div class="single-input"><input type="text" v-model="nazwisko"></div>
        <div class="single-input"><input type="text" v-model="klasa"></div>
        <div class="single-input">
          <select v-model="temat">
            <option selected disabled></option>
            <option>#temat1</option>
            <option>#temat2</option>
            <option>#temat3</option>
            <option>#temat4</option>
          </select>
        </div>
        <div class="single-input"><input type="text" v-model="email"></div>
      </div>
    </div>
    <div class="button">
      <button>Zapisz się!</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Etap2",
  data() {
    return {
      imie: '',
      nazwisko: '',
      klasa: '',
      temat: '',
      email: ''
    }
  }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Lato:400,700,900&display=swap');


  .container {
    background-color: #1E000E;
    color: rgb(235, 181, 33);
    font-family: Lato;
    text-transform: uppercase;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    font-weight: 900;
    padding-bottom: 4rem;

    .title {
      width: 100%;
      height: 6rem;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 40px;
    }
    .main {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: row;
      width: 40vw;
      height: 20em;
      margin-left: 2.5rem;

      .left {
        width: 30%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;

        .single-name {
          width: 10rem;
          height: 3rem;
          text-align: left;
        }
      }
      .right {
        width: 70%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;

        .single-input {
          width: 20rem;
          height: 3rem;
          display: flex;
          justify-content: flex-end;
          input {
            border-radius: 10px;
            background-color: rgb(54, 10, 31);
            border: none;
            width: 20vw;
            height: 2vw;
            color: white;
            font-size: 1.1rem;
            outline: none;
            padding-left: 1vw;
          }
          select {
            border-radius: 10px;
            background-color: rgb(54, 10, 31);
            border: none;
            width: 21vw;
            height: 2vw;
            color: white;
            font-size: 1.3rem;
            outline: none;
              -moz-appearance:none; /* Firefox */
              -webkit-appearance:none; /* Safari and Chrome */
              appearance:none;
          }
        }
      }
    }
    .button {
      display: flex;
      width: 60vw;
      justify-content: flex-end;
      padding-right: 20vw;
      
      button {
        border-radius: 18px;
        background-color:rgb(235, 181, 33);
        border: 1px solid rgb(235, 181, 33);
        font-family: Lato;
        font-weight: 900;
        text-transform: uppercase;
        height: 3rem;
        width: 10rem;
        font-size: 2.5vh;
        outline: none;
      }
    }
  }
</style>