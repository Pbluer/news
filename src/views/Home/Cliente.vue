<template>
  <div class="cliente-review">
    <h1>CLIENTE TESTIMONIALS</h1>
    <div class="review">

      <div>
        <img src="../../assets/images/image-emily.jpg" alt="Emily">
        <h3>We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</h3>
        <h2>Emily R.</h2>
        <p>Marketing Director</p>
      </div>

      <div>
        <img src="../../assets/images/image-thomas.jpg" alt="Thomas">
        <h3>Sunnyside's enthusiasm couple with their keen interest in our brand's success made it a satisfying and enjoyable experience.</h3>
        <h2>Thomas S.</h2>
        <p>Chief Operation Officer</p>
      </div>

      <div>
        <img src="../../assets/images/image-jennie.jpg" alt="Jennie">
        <h3>Incredible and result! Our sales increased over 400% when we worked with Sunnyside. Highly recomended!</h3>
        <h2>Jennie F.</h2>
        <p>Business Owner </p>
      </div>

    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>

  .cliente-review {   
  
    h1 {
      font-family: 'Fraunces';
      text-align: center;
      font-size: 1.5rem;
      color: rgb(130, 130, 130);
      letter-spacing: 5px;
      margin: 30px 0;
    }

    .review {
      display: flex;
      flex-direction: row;
      padding: 0 10%;    

      div {
        text-align: center;
        margin: 0 30px 150px 30px;
      

        img{
          border-radius: 100%;
          width: 20%;
          margin: 50px 0;
        }

        h3 {
          margin: 20px 0;
          color: rgb(73, 73, 73);
        }

        h2 {
          font-family: 'Fraunces';
          margin: 50px 0 0 0;
        }

        p {
          margin: 0;
          font-size: .9rem;
          color: rgb(130, 130, 130);
        }

      }

    }

  }

</style>