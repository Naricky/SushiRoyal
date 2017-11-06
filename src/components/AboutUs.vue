<template>
  <div>
    <div class="backgroundAboutUsImage">
      <div class="catchyTitle"> ͏Ab͏o͏u͏t ͏Us</div>
        <div class="descriptionBox">
        <p class="descriptionTitle"> It started with simple dream</p>
        <p class="descriptionDetail"> It was thirty years ago when Chef Choi started eating sushi. He likes sushi. He started making sushi. He lovesss sushi.</p>
        </div>
        <div class="descriptonBox2">
          <img class="imageAboutUs" src="../assets/sushi.png"></img>
        </div>
    </div>

  </div>
</template>

<script>
export default {

}
</script>


<style scoped>

  p {
    font-family: serif;
    margin-left: 150px;
  }
  .descriptionBox {
    margin-top: 50px;
    padding-right: 250px;
    float: left;
  }

  .imageAboutUs {
    margin-top: 50px;
  }

  .descriptionBox2 {
    margin-right: 150px;
  }

  .descriptionTitle {
    font-size: 30px;
    font-weight: bold;


  }

  .descriptionDetail {
    font-size: 20px;
    font-style: italic;
    width: 500px;


  }

  .backgroundAboutUsImage {
    height: 500px;
  opacity: 1;
  background: url("../assets/aboutusback.jpg") no-repeat center center fixed;
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


</style>


