<template>
  <div>
    <div class="backgroundGalleryImage">
      <div class="catchyTitle"> ͏Gallery </div>
      <!-- <div v-for="number in [currentNumber]" transition="fade">
        <img class='yum' :src="yum[currentNumber % yum.length]  " />
      </div> -->
      <hr>
        <div class="descriptionBox">
          <figure>
            <!-- <img class="food" src="../assets/3.jpg" />
            <img class="food" src="../assets/4.jpg" />
            <img class="food" src="../assets/6.jpg" />
            <img class="food" src="../assets/7.jpg" /> -->
            <img class="food" src="../assets/DSC00012-2.jpg" />
            <img class="food" src="../assets/DSC00024.jpg" />
            <img class="food" src="../assets/DSC00031.jpg" />
            <img class="food" src="../assets/DSC00038.jpg" />
            <img class="food" src="../assets/DSC00092.jpg" />
            <img class="food" src="../assets/DSC00094.jpg" />
            <img class="food" src="../assets/DSC00135.jpg" />
            <img class="food" src="../assets/DSC00149.jpg" />
            <img class="food" src="../assets/DSC00196.jpg" />
            <img class="food" src="../assets/DSC00221.jpg" />
            <img class="food" src="../assets/DSC00284.jpg" />
            <img class="food" src="../assets/DSC00292.jpg" />
          </figure>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  // data () {
  //   return {
  //      yum: [require('../assets/DSC00012-2.jpg'), require('../assets/DSC00024.jpg'), require('../assets/DSC00031.jpg'), require('../assets/DSC00038.jpg'), require('../assets/DSC00092.jpg'), require('../assets/DSC00094.jpg'), require('../assets/DSC00122.jpg'), require('../assets/DSC00135.jpg'), require('../assets/DSC00149.jpg'), require('../assets/DSC00161.jpg'), require('../assets/DSC00196.jpg'), require('../assets/DSC00221.jpg'), require('../assets/DSC00284.jpg'), require('../assets/DSC00292.jpg'),],
  //       currentNumber: 0
  //   }
  // },
  // beforeMount()  {
  //       this.startRotation();
  //   },

  //   methods: {
  //       startRotation: function() {
  //           this.timer = setInterval(this.next, 6000);
  //           console.log('rotation happens')
  //       },

  //       stopRotation: function() {
  //           clearTimeout(this.timer);
  //           this.timer = null;
  //       },

  //        next: function() {
  //           this.currentNumber += 1
  //       }

  //   }
}
</script>


<style scoped>

  .backgroundGalleryImage {
    /*background-color: #F5F5EC;*/
    background-color: black;
    height:550px;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
  }

  .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;
  }

  .food {
    height: 15%;
    width: 15%;
  }
</style>


