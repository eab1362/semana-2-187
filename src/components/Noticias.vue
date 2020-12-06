<template>
  <div class="container-fluid">
    <div class="row">
      <div
        class="col-sm-6"
        style="background-color: lavender height: 800px"
        v-for="(noti, index) of noticias"
        :key="index"
      >
        <div class="card" style="width: 400px height:600px"  >
          <img class="card-img-top" width= "300px" height= "200px" :src="noti.urlToImage" alt="Card image" />
          <div class="card-body" style="height: 200px">
            <h4 class="card-title">{{noti.title}}</h4>
            <p class="card-text">{{noti.description}}</p>"
            <a v-bind:href="noti.url" class="btn btn-primary">Saber más</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import Items from "./Items.vue";

export default {
  components: { Items },
  name: "Noticias",
  props: {
    msg: String,
  },
  data() {
    return { noticias: null };
  },

  mounted() {
    axios
      .get(
        "http://newsapi.org/v2/top-headlines?country=co&apiKey=b56575f5563249df9f5cf440528e0191&pageSize=4"
      )
      .then((response) => {
        this.noticias = response.data.articles;
        console.log(this.noticias);
      });
  },
};
</script>



