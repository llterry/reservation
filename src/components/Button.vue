<template>
    <div class="button">
          <button v:style="btn" class="btn">Click to Reserve</button>
        </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
  .button {
    width: 100%;
    height: 50px;
    font-size: 19px;
    font-family: monospace;
    text-align: center;
    /*background: #FFF;*/
    color: #313131;
    border-color: #313131;
  }

  .btn {
    cursor: pointer;
    /*display: block;*/
    padding: 10px;
    max-width: 100%;
    max-height: 100%;
    outline: none;
    background-color:rgb(245, 141, 99);
    border-radius: 10px;

  }

  .btn:hover {
    background-color: rgb(242, 196, 178);
  }

  .btn:active {
    background-color: rgb(247, 93, 31);
  }
/*  sass code, need to install sass (npm install -g sass)
  .btn:hover {
      background-color: lighten($color: rgb(245, 141, 99), $amount: 10);
  }
    .btn:active {
       background-color: darken($color: rgb(245, 141, 99), $amount: 5);
    }
    */
</style>