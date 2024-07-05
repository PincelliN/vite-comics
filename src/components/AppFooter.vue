<script>
export default{
    name:"AppFooter",
    data() {
    return {
      links: [{
        text: "characters",
        url: "#",
        state: false,
      },
      {
        text: "comics",
        url: "#",
        state: true,
      },
      {
        text: "movies",
        url: "#",
        state: false,
      },
      {
        text: "tv",
        url: "#",
        state: false,
      },
      {
        text: "games",
        url: "#",
        state: false,
      },
      {
        text: "collectibles",
        url: "#",
        state: false,
      },
      {
        text: "videos",
        url: "#",
        state: false,
      },
      {
        text: "fans",
        url: "#",
        state: false,
      },
      {
        text: "news",
        url: "#",
        state: false,
      },
      {
        text: "shop",
        url: "#",
        state: false,
      },
      ]
    }
  }
}
</script>
<template>
    <div class="list-box">
        <div>
            <h4>dc comics</h4>
            <ul>
                <li v-for="link in links"> <a :href="link.url"></a>{{ link.text }}</li>   
            </ul>
            <div>
                <h4>Shop</h4>
                <ul>
                    <li><a href="#"></a>Shop DC</li>
                    <li><a href="#"></a>Shop DC collectibles</li>
                </ul>
            </div>
        </div>
        <div>
            <h4>dc</h4>
            <ul>
                <li><a href="#"></a>Terms of Use</li>
                 <li><a href="#"></a>Privacy policy(New)</li>
                  <li><a href="#"></a>Ad Choices</li>
                   <li><a href="#"></a>Advertising</li>
                    <li><a href="#"></a>Jobs</li>
                     <li><a href="#"></a>Subscriptions</li>
                      <li><a href="#"></a>Talent Workshops</li>
                       <li><a href="#"></a>CPSC Certificateas</li>
                        <li><a href="#"></a>Rating</li>
                         <li><a href="#"></a>Shop Help</li>
                          <li><a href="#"></a>Contacts Us</li>
            </ul>
        </div>
        <div>
            <h4>sites</h4>
            <ul>
                <li><a href="#"></a>DC</li>
                <li><a href="#"></a>MAD Magazine</li>
                <li><a href="#"></a>Dc Kids</li>
                <li><a href="#"></a>DC Universe</li>
                <li><a href="#"></a>DC Power Visa</li>
            </ul>
        </div>

    </div>
    <footer>
        <button>Sing-up Now</button>
         
        <div>
            <h3>Follow us</h3>
            <ul>
                <li><a href="#"><img src="../assets/footer-facebook.png" alt=""></a></li>
                <li><a href="#"><img src="../assets/footer-twitter.png" alt=""></a></li>
                <li><a href="#"><img src="../assets/footer-youtube.png" alt=""></a></li>
                <li><a href="#"><img src="../assets/footer-pinterest.png" alt=""></a></li>
                <li><a href="#"><img src="../assets/footer-periscope.png" alt=""></a></li>
               
            </ul>
        </div>
    </footer>
</template>
<style scoped>
.list-box{
    display: flex;
    justify-content: flex-start;
    gap: 10px;
    background-image:url(../assets/dc-logo-bg.png),url(../assets/footer-bg.jpg);
    background-size: contain,cover;
     background-position-x: 70%;
     background-repeat: no-repeat;
     padding: 10px;

    h4{
        color: white;
        text-transform: uppercase;
        font-weight: bolder;
        text-align: start;
    }
    ul{
        color: rgb(168, 168, 168);
        list-style: none;
        text-align: start;
        text-transform: capitalize;
    }
}

footer{
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: black;
    div{
        display: flex;
        justify-content: flex-start;
           align-items: center;
        ul{
            display: flex;
            justify-content: flex-start;
            list-style: none;
               align-items: center;
            li{
                margin: 1rem;
            }
        }
    }
}
</style>