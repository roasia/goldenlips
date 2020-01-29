<template>
  <div class="container">
    <div class="row" v-if="!sendSucced && !loading && !error">
      <vote @clicked="clicked" v-for="item in array" :key="item._id" :name="item.presentation" :id="item._id" :votes="item.votes"/>
    </div>
    <div class="send" v-if="sendSucced && !error">
      Dziękujemy za oddanie głosu!
    </div>
    <div class="send" v-if="error">
      Głos z tego adresu już został policzony
    </div>
    <div class="send" v-if="loading">
      <Loading/>
    </div>
  </div>
</template>

<script>
import axios from 'axios'

import vote from '@/components/vote'
import Loading from '@/components/LoadingCircle'

export default {
  name: 'etap3',
  components: {
    vote,
    Loading
  },
  data() {
    return {
      sendSucced: false,
      error: false,
      loading: false,
      array: []
    }
  },
  methods: {
    clicked(id) {
      this.loading = true;
      axios({
        method: 'post',
        url: 'http://localhost:5000/presentation/vote',
        data: {
          "_id": id
        }
      }).then(() => {
        this.loading = false;
        this.sendSucced = true;
      }).catch(() => {
        this.loading = false;
        this.error = true;
      });
    }
  },
  created() {
    axios({
      method: 'post',
      url: 'http://localhost:5000/presentation/all'
    }).then(response => {
      this.array = response.data.presentations;
    });
  }
}
</script>

<style lang="scss" scoped>
.container {
  background-color: #1E000E;
  color: #ddab40;
  font-family: Lato;
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: column;
  padding-bottom: 4rem;
  align-items: center;

  .row {
    width: 70vw;
    height: auto;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: auto;
    grid-row-gap: 2.7rem;
  }

  .send {
    width: 70vw;
    height: 29rem;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 3rem;
  }
}
</style>