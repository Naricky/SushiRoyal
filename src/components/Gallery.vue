<template>
  <div>
    <div class="backgroundGalleryImage">
      <div class="catchyTitle"> ͏Gallery </div>

      <hr>
        <div class="descriptionBox">
          <figure>
            <img class="food" src="../assets/DSC00012-2.jpg" />
            <!-- TODO for Kevin: If all the pictures are enlisted with HD, there seems like runtime problem. ( It takes about 20 seconds to load the page. This is too much. If you test out with one picture with google dev tool ( go to network, and when you load the page, it will show how much seconds which components are taking too long. Main problem here are pictures are of too high quality which takes up about ~20mb per picture. https://stackoverflow.com/questions/4504497/how-to-reduce-size-of-largeish-image-for-web-page-download   Couple of solutions here. For now, I've removed pictures so it runs smoothly on local machine.)) -->
          </figure>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {

    }
  },
    methods: {

    }
}
</script>


<style scoped>

  .backgroundGalleryImage {
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


