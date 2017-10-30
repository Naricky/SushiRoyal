<template>
  <div>
    <div class="backgroundAboutUsImage">
      <div class="catchyTitle"> ABOUT US HERE</div>
        <div class="descriptionBox">
        <p class="descriptionTitle"> It started with simple dream...</p>
        <p class="descriptionDetail"> Namwook loves Sushi. He started making Sushi.</p>
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
    float: right;
  }

  .descriptionTitle {
    font-size: 30px;
    font-weight: bold;
    font-family: arial;

  }

  .descriptionDetail {
    font-size: 20px;
    font-style: italic;
    font-family: arial;

  }

  .backgroundAboutUsImage {
    background-color: white;
    height:550px;
  }

  .catchyTitle {
    padding-top: 110px;
    text-align: center;
    font-size: 80px;
  }


</style>


