<template>
  <div>
    <div class="backgroundMenuImage">
      <div class="catchyTitle"> Menu</div>
      <hr>
      <body>
  <h1>Favorites</h1>
    <div class="description">
      <image-slider>
        <p>
          <a @click="prev">Previous</a> || <a @click="next">Next</a>
        </p>
        <div v-for="number in [currentNumber]"
             transition="fade">
          <img
              :src="images[Math.abs(currentNumber) % images.length]"
              v-on:mouseover="stopRotation"
              v-on:mouseout="startRotation"
          />
        </div>
      </image-slider>
    </div>
    
    <!-- <img class="food" src="../assets/menu1.jpg" />
    <img class="food" src="../assets/menu2.jpg" /> -->
        <!-- <p>Ins: deep fried avocado, spicy tuna</p>
        <p>Top: unagi, house wine, spicy mayo, yam flake, sauce</p> -->
        

        <!-- <h2> Monkey Brain Roll </h2>
        <img class="food" src="../assets/DSC00012-2.jpg" />
        <h2> Crispy Roll </h2>
        <img class="food" src="../assets/DSC00031.jpg" />
        <h2> Red Dragon Roll </h2>
        <img class="food" src="../assets/DSC00092.jpg" />
        <h2> Crunch Roll </h2>
        <img class="food" src="../assets/DSC00094.jpg" />
        <h2> Canucks Roll </h2>
        <img class="food" src="../assets/DSC00149.jpg" /> -->
    
    <!-- <tr>
      <td>  
        
      </td>
      <td>
        <h2>Miso Soup</h2>
Five large shrimp served with our zesty cocktail sauce $6.95
      </td>
      <td>
        <h2>Crab Cakes</h2>
Homemade crab cakes with tender lump crab meat and just the right amount of spices and seasonings served with Remoulade sauce $7.95
      </td>

    </tr>
    <tr>
      <td>
        <h2>Artichoke French</h2>
Egg-battered and served in a sherry, butter & lemon sauce $6.95
      </td>
      <td>
        <h2>Shrimp Alexander</h2>
Jumbo shrimp wrapped in bacon and topped with melted Feta $7.95</td>
    </tr>
    <tr>
      <td>
        <h2>Artichokes Alexander</h2>
Artichokes wrapped in bacon and topped with melted Feta cheese $6.95
      </td>
      <td>
        <h2>Southern Fried Asparagus</h2>
Lightly battered & deep fried, served with Ranch dressing $5.95
      </td>
    </tr>
    <tr>
      <td>
        <h2>Mozzarella Sticks</h2>
Mozarella cheese, lightly battered and deep-fried, served with our traditional red sauce $5.95
      </td>
      <td>
        <h2>Garlic Bread</h2>
Topped with Mozarella and served with our traditional red sauce $4.95
      </td>
    </tr>
    <tr>
      <td>
        <h2>Chicken Tenders</h2>
Marinated tenderloins covered with our special mildly spiced breadcrumbs, deep-fried to a golden brown & served with dipping sauce $5.95
      </td>
    </tr> -->
  <div class="download">
          <p>
             <a href="../assets/takeout.pdf" class="button" download>Download Menu</a>
          </p>
  </div>
      </body>
   </div>
 </div>
</template>

<script>
export default {
  data () {
    return {
      el: 'image-slider',
      data: {
          images: [require('../assets/DSC00012-2.jpg'), require('../assets/DSC00031.jpg'), require('../assets/DSC00092.jpg'), require('../assets/DSC00094.jpg'), require('../assets/DSC00149.jpg')],
          currentNumber: 0
      },
    }
  },
  ready: function () {
        this.startRotation();
    },

  methods: {
        startRotation: function() {
            this.timer = setInterval(this.next, 3000);
        },

        stopRotation: function() {
            clearTimeout(this.timer);
            this.timer = null;
        },

        next: function() {
            this.currentNumber += 1
        }
  }
}
</script>


<style scoped>

  .backgroundMenuImage {
    height: 500px;
    width: 100%;
  /*opacity: 1;
  background: url("../assets/menuback.jpg") no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;*/
    background-color: white;

  }

   .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;
  }

   .food {
    height: 35%;
    width: 30%;

   }

  .fade-transition {
  transition: all 0.8s ease;
  overflow: hidden;
  visibility: visible;
  opacity: 1;
  position: absolute;
  }
  
  .fade-enter, .fade-leave {
  opacity: 0;
  visibility: hidden;
  }

</style>


