<template>
    <div class="backgroundGalleryImage">
      <div class="catchyTitle"> ͏Gallery </div>
      <hr>
        <body>
         <coverflow :coverList="coverList" :coverWidth="260" :index="2" bgColor="#333"></coverflow>
        </body>
    </div>
</template>

<script>
import Coverflow from './slider/Coverflow'

export default {
   name: 'app',
    data () {
      return {
        coverList: [
          {
            cover: require('../assets/DSC00012-2.jpg'),
            title: 'Monkey Brain Roll'
          }, {
            cover: require('../assets/DSC00031.jpg'),
            title: 'Crispy Roll'
          }, {
            cover: require('../assets/DSC00092.jpg'),
            title: 'Red Dragon Roll'
          }, {
            cover: require('../assets/DSC00094.jpg'),
            title: 'Crunch Roll'
          }, {
            cover: require('../assets/DSC00149.jpg'),
            title: 'Canucks Roll'
          }
        ],
      }
    },
    components: {
      Coverflow
    }
}

</script>

<style scoped>

  body {
    background-color: black;
  }

  .backgroundGalleryImage {
    background-color: black;
    height: 100%;
    width: 100%;
  }

  .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;
  }

  .images {
    height: 75%;
    width: 75%;
  }

</style>
