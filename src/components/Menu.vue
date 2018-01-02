<template>
  <div>
    <div class="backgroundMenuImage">
      <div class="catchyTitle"> Menu</div>
      <hr>
        <body>
           <div>
    <gallery :images="images" :index="index" @close="index = null"></gallery>
    <div
      class="image"
      v-for="(image, imageIndex) in images"
      :key="imageIndex"
      @click="index = imageIndex"
      :style="{ backgroundImage: 'url(' + image + ')', width: '300px', height: '200px' }"
    ></div>
  </div>
          <!-- <coverflow :coverList="coverList" :coverWidth="260" :index="2"></coverflow> -->
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
import VueGallery from './slider/gallery';

export default {
    data: function () {
      return {
        images: [
          require('../assets/DSC00012-2.jpg'),
          require('../assets/DSC00031.jpg'),
          require('../assets/DSC00092.jpg'),
          require('../assets/DSC00094.jpg'),
          require('../assets/DSC00149.jpg'),
          require('../assets/menu1.jpg'),
          require('../assets/menu2.jpg')
        ],
        index: null
      };
    },
 
    components: {
      'gallery': VueGallery
    },
  }
// import Coverflow from './slider/Coverflow'

// export default {
//  name: 'app',
//     data () {
//       return {
//         coverList: [
//           {
//             cover: require('../assets/DSC00012-2.jpg'),
//             title: 'Monkey Brain Roll'
//           }, {
//             cover: require('../assets/DSC00031.jpg'),
//             title: 'Crispy Roll'
//           }, {
//             cover: require('../assets/DSC00092.jpg'),
//             title: 'Red Dragon Roll'
//           }, {
//             cover: require('../assets/DSC00094.jpg'),
//             title: 'Crunch Roll'
//           }, {
//             cover: require('../assets/DSC00149.jpg'),
//             title: 'Canucks Roll'
//           }, {
//             cover: require('../assets/menu1.jpg'),
//             title: 'Menu'
//           }, {
//             cover: require('../assets/menu2.jpg'),
//             title: 'Menu'
//           }
//         ],
        
//         codeOne: `
//         <coverflow :coverList="coverList" :coverWidth="260" :index="2" bgColor="#ddd"></coverflow>
//         `,
       
//       }
//     },
//     components: {
//       Coverflow
//     }
// }
</script>


<style scoped>

  .backgroundMenuImage {
    height: 500px;
    width: 100%;
    background-color: white;
  }

   .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;
  }

   .images {
    height: 50%;
    width: 50%;
   }

  


</style>


