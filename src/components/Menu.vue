<template>
  <div>
    <div class="backgroundMenuImage">
      <div class="catchyTitle"> Menu</div>
      <hr>
      <body>
  <h1>Favorites</h1>
   <!-- TODO for Kevin: So I retrieved back Menu template. This would be really good practice for you so I left it blank with basic datset structure and instructions in case you get lost.. ( Seems like you were going to build html file for all the rolls, but that is not optimum.)

  a) You can populate images and descriptions using v-for. Example would be:
    <aa v-for="response in responsess">
        {{response.answer}}</aa>. It's not foreach for vue. Vue doc has great read on it. Once you populate these vue dataset structure..
  b) https://vuejs.org/v2/examples/modal.html
     What you are trying to do is called 'modal' ; in simple, a popup box. This allows you to do what you described to me in regards menus. Quite straight forward ; play around with the example given above.
  c) When you make your first modal work, make sure to wrap them with specific class/id to make sure one css applies to all modals. Always practie DRY coding ( although, I wasn't aware of this when this side project was started lol).

     -->
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
      images: [require('../assets/DSC00012-2.jpg'), require('../assets/DSC00031.jpg'), require('../assets/DSC00092.jpg'), require('../assets/DSC00094.jpg'), require('../assets/DSC00149.jpg')],

     descriptions:  [
                      [ { id: 1, description :'description 1'},
                        { id: 2, description :'description 2'},
                        { id: 3, description :'description 3'},
                        { id: 4, description :'description 4'},
                        { id: 5, description :'description 5'},
                      ],
                    ],
    }
  },

  methods: {

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


