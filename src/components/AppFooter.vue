<script>
export default {
  name: "AppFooter",
  data() {
    return {
      shopAreas: [{
        area: "Dc Comics",
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

        ]
      },
      {
        area: "Shop",
        links:
          [{
            text: "Shop Dc",
            url: "#",
            state: false,
          },
          {
            text: "Shop Dc Collectibles",
            url: "#",
            state: true,
          }]
      },
      {
        area: "Dc",
        links:
          [{
            text: "Terms of Use",
            url: "#",
            state: false,
          },
          {
            text: "Privacy policy(New)",
            url: "#",
            state: true,
          },
          {
            text: "Ad Choices",
            url: "#",
            state: false,
          },
          {
            text: "Advertising",
            url: "#",
            state: false,
          },
          {
            text: "Jobs",
            url: "#",
            state: false,
          },
          {
            text: "Subscriptions",
            url: "#",
            state: false,
          },
          {
            text: "Talent Workshops",
            url: "#",
            state: false,
          },
          {
            text: "CPSC Certificateas",
            url: "#",
            state: false,
          },
          {
            text: "Rating",
            url: "#",
            state: false,
          },
          {
            text: "Shop Help",
            url: "#",
            state: false,
          },
          {
            text: "Contacts Us",
            url: "#",
            state: false,
          }]
      },
      {
        area: "Sites",
        links: [{
          text: "Dc",
          url: "#",
          state: false,
        },
        {
          text: "MAD Magazine",
          url: "#",
          state: true,
        },
        {
          text: "Dc Kids",
          url: "#",
          state: false,
        },
        {
          text: "Dc Universe",
          url: "#",
          state: false,
        },
        {
          text: "Dc Power Visa",
          url: "#",
          state: false,
        }
        ]
      }
      ],

    }
  }
}
</script>
<template>
  <div class="back">
    <div class="list-box">
      <div v-for="shoparea in shopAreas">
        <h4>{{ shoparea.area }}</h4>
        <ul>
          <li v-for="link in shoparea.links"> <a :href="link.url"></a>{{ link.text }}</li>
        </ul>
      </div>
    </div>
  </div>
  <footer>
    <section>
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
    </section>
  </footer>
</template>


<style scoped>
.back {
  background-image: url(../assets/footer-bg.jpg);
  background-size: cover;

  background-repeat: no-repeat;


  .list-box {
    background-image: url(../assets/dc-logo-bg.png);
    background-size: 40%;
    background-position: 100% 50%;
    background-repeat: no-repeat;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    align-content: flex-start;
    flex-wrap: wrap;
    height: 294px;
    width: 80%;
    margin: 0 auto;
    padding: 10px;
    gap: 10px;



    div {
      margin-top: 10px;




      h4 {
        color: white;
        text-transform: uppercase;
        font-weight: bolder;
        margin-bottom: 5px;
      }

      ul {
        color: rgb(168, 168, 168);
        list-style: none;
        text-transform: capitalize;



      }
    }
  }
}

footer {

  background-color: black;

  section {
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    button {
      background-color: black;
      border: 1px solid blue;
      padding: 5px;
      color: white;
      text-transform: uppercase;
    }

    div {
      display: flex;
      justify-content: flex-start;
      align-items: center;

      h3 {
        color: blue;
        text-transform: uppercase;
      }

      ul {
        display: flex;
        justify-content: flex-start;
        list-style: none;
        align-items: center;
        gap: 8px;
        padding: 10px;


        img {
          width: 25px;
        }

      }
    }
  }
}
</style>