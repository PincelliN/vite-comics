<script>
export default{
    name:"AppShopInfo",
    data() {
    return {
      infos: [{
        url:"../assets/buy-comics-digital-comics.png",
        testo:"Digital Comics"
      },{
        url:"../assets/buy-comics-merchandise.png",
        testo:"Dc Merchandise"
      },
      {
        url:"../assets/buy-comics-shop-locator.png",
        testo:"Subsciption"
      },
      {
        url: "../assets/buy-comics-subscriptions.png",
        testo:"Comic Shop Locator"
      },
      
      {
        url:"../assets/buy-dc-power-visa.svg",
        testo:"dc power visa"
      }  
      ]
    }
  }
}
</script>

<template>
<div>
    <ul>
        <li v-for="info in infos"><a href="#"><img :src="info.url" :alt="info.testo"></a>{{ info.testo }}</li>
    </ul>
</div>
</template>
<style scoped>
div{
    background-color: cornflowerblue;
    color: white;
    ul{
        width: 80%;
        display: flex;
        justify-content: space-around;
    }
}
</style>