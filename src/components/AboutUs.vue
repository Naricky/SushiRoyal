<template>
  <div>
    <div class="backgroundAboutUsImage">
      <div class="catchyTitle"> ͏Ab͏o͏u͏t ͏Us</div>
      <hr>
        <div class="descriptionBox">
        <p class="descriptionTitle"> Ganso's Story</p>
        <p class="descriptionDetail"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent hendrerit risus vitae semper accumsan. Suspendisse efficitur dui vitae leo ornare placerat. Curabitur tempus euismod ante vel finibus. Nam euismod ipsum eget tellus dictum, a dictum nulla consectetur. Nam condimentum pulvinar dui sit amet dignissim. Proin ac tellus non quam condimentum aliquam ac vel nunc. Ut ut mi consequat, tempus velit vel, tincidunt diam. Ut et lacus erat. Nullam tristique nisi egestas, tristique leo nec, mattis est. Cras lobortis eu magna eget suscipit. Sed et nisi sed risus luctus blandit. Nullam sed ex dui.</p>
        </div>
        <div class="descriptonBox2">
          <img class="imageAboutUs" src="../assets/chef.jpg"></img>
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
    padding-right: 100px;
    float: left;
  }

  .imageAboutUs {
    margin-top: 50px;
    float:right;
    height: 300px;
    width: 300px;
    margin-right: 150px;
  }

  .descriptionBox2 {
    margin-right: 150px;
  }

  .descriptionTitle {
    font-size: 30px;
    font-weight: bold;

  }

  .descriptionDetail {
    font-size: 15px;
    font-style: italic;
    width: 500px;


  }

  .backgroundAboutUsImage {
  height: 500px;
  opacity: 1;
  /*background: url("../assets/aboutusback.jpg") no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;*/
background-color: #FFF;
  }

  .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;

  }


</style>


