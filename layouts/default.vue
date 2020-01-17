<template>
  <div>
    <Header />
    <nuxt />
    <Footer />
  </div>
</template>
<script>
import Header from '@/components/header'
import Footer from '@/components/footer'
export default {
  data () {
    return {
      
    }
  },
  components:{
    Header,Footer
  }
}
</script>
<style lang="less">
  * {
     margin: 0;
     padding: 0;
     box-sizing: border-box;  
  }
  a {
    text-decoration: none;
    color: #000;
    
  }
</style>