<template>
<section>
  <Header />
  <div class="content">
    <div class="content__container">
      <Headline :title="title" :image="image" :benefit="benefit" :advantages="advantages" />
      <Request />
      <Contacts />
    </div>
  </div>
  <Footer />
</section>
</template>

<script>
import jsonData from '../data.json'
import Header from "@/components/Header";
import Headline from "@/components/Headline";
import Request from "@/components/Request";
import Contacts from "@/components/Contacts";
import Footer from "@/components/Footer";

export default {
  components: { Header, Headline, Request, Contacts, Footer },
  methods: {
    getLanding(path){ 
      return jsonData.landings.find(landing => landing.path === path)
    }, 
    getAdvantages(name){
      return jsonData.advantages.find(advantages => advantages.name === name).list
    }
  },
  computed: {
      title(){
        return this.getLanding(this.$route.params.landing).title
      },
      image(){
        return this.getLanding(this.$route.params.landing).image
      },
      benefit(){
       return this.getLanding(this.$route.params.landing).benefit
      },
      advantages(){
        return this.getAdvantages(this.getLanding(this.$route.params.landing).advantages)
      }
  },
};
</script>

<style>
.content {
  display: flex;
  overflow: hidden;
  justify-content: center;
}

.content__container {
  display: flex;
  overflow: hidden;
  flex-direction: column;
  justify-content: center;
  width: 1120px;
  padding: 20px 10px;
}
</style>