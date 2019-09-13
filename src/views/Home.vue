<template>
  <div class="home">
    <div class="solid-container" style="height:100vh">
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import testpdf from "@/assets/pdf/CondoLiving.pdf";
// import flipbook from "@/config/3dflipbook.min.js";



export default {
  name: "home",
  components: {
    HelloWorld
  },
  data(){
    return{
      testpdf:testpdf,
    }
  },
  created(){
    $('.solid-container').FlipBook({pdf: this.testpdf});
  }
};
</script>
