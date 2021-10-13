<template>
  <main>
    <div class="container-show">
      <div class="brand">
        <h2>Transforme your brand</h2>

        <p>
          we are a full service creative agency specializing in helping brands
          grow fast. Engage your clients through compelling visuals that do most
          of the marketing for you.
        </p>

        <a href="#">LEARN MORE</a>
      </div>

      <div class="egg-img"></div>

      <div class="cup-img"></div>

      <div class="audience">
        <h2>Stand out to the right audience</h2>

        <p>
          Using a collaborative formula of designers, researchers,
          photographers, videographers, and copywriters, we'll build and extend
          your brand in digital places.
        </p>

        <a href="#">LEARN MORE</a>
      </div>

      <div class="cherry-img">
        <h2>Graphic Design</h2>
        <p>Great design makes you memorable. We deliver artwork that underscores your brand massage and captures potential client's attention.</p>
      </div>

      <div class="orange-img">
        <h2>Photography</h2>
        <p>Increase your credibility by getting the most stunning, high-quality that improve your business image.</p>
      </div>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
.container-show {
  display: grid;
  grid-template-columns: 1fr 1fr;

  .brand {
    padding: 30% 0 0 10%;
    text-align: left;

    h2 {
      width: 400px;
      font-size: 2.5rem;
      color: rgb(38, 38, 38);
      font-family: "Fraunces";
      margin-bottom: 10px;
    }

    p {
      width: 600px;
      color: rgb(58, 58, 58);
      margin-bottom: 15px;
    }

    a {
      font-family: "Fraunces";
      color: rgb(38, 38, 38);
      text-decoration: underline 3px #fdd302;
    }
  }

  .egg-img {
    min-height: 87vh;
    width: 100%;
    background-image: url("../../assets/images/desktop/image-transform.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
  }

  .cup-img {
    min-height: 87vh;
    width: 100%;
    background-image: url("../../assets/images/desktop/image-stand-out.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
  }

  .audience {
    padding: 30% 0 0 10%;
    text-align: left;

    h2 {
      width: 400px;
      font-size: 2.5rem;
      color: rgb(38, 38, 38);
      font-family: "Fraunces";
      margin-bottom: 10px;
    }

    p {
      width: 600px;
      color: rgb(58, 58, 58);
      margin-bottom: 15px;
    }

    a {
      font-family: "Fraunces";
      color: rgb(38, 38, 38);
      text-decoration: underline 3px #fe7263;
    }
  }

  .cherry-img {
    min-height: 87vh;
    width: 100%;
    background-image: url("../../assets/images/desktop/image-graphic-design.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
    text-align: center;
    padding: 55% 20% 20%;

    h2 {
      font-family: "Fraunces";
      font-size: 1.5rem;
      color: #278575;
    }

    p {
      color: rgb(63, 158, 142)
    }

  }
  

  .orange-img {
    min-height: 87vh;
    width: 100%;
    background-image: url("../../assets/images/desktop/image-photography.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
    text-align: center;
    padding: 55% 20% 20%;

    h2 {
      font-family: "Fraunces";
      font-size: 1.5rem;
      color: #1c6187;
    }

    p {
      color: #1779ae;
    }

  }
}

@media screen and ( min-width:375px ) {
  .container-show {
  display: grid;
  grid-template-columns:1fr;

  .brand {
    padding: 10%;
    text-align: center;

    h2 {
      width: 200px;
      font-size: 2rem;
      color: rgb(38, 38, 38);
      font-family: "Fraunces";
      margin-bottom: 10px;
    }

    p {
      width: 600px;
      color: rgb(58, 58, 58);
      margin-bottom: 15px;
    }

    a {
      font-family: "Fraunces";
      color: rgb(38, 38, 38);
      text-decoration: underline 3px #fdd302;
    }
  }

  .egg-img {
    min-height: 87vh;
    width: 50%;
    background-image: url("../../assets/images/desktop/image-transform.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
  }

  .cup-img {
    min-height: 87vh;
    width: 50%;
    background-image: url("../../assets/images/desktop/image-stand-out.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
  }

  .audience {
    padding: 5% 0 0 5%;
    text-align: left;

    h2 {
      width: 200px;
      font-size: 2.5rem;
      color: rgb(38, 38, 38);
      font-family: "Fraunces";
      margin-bottom: 10px;
    }

    p {
      width: 600px;
      color: rgb(58, 58, 58);
      margin-bottom: 15px;
    }

    a {
      font-family: "Fraunces";
      color: rgb(38, 38, 38);
      text-decoration: underline 3px #fe7263;
    }
  }

  .cherry-img {
    min-height: 87vh;
    width: 50%;
    background-image: url("../../assets/images/desktop/image-graphic-design.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
    text-align: center;
    padding: 55% 20% 20%;

    h2 {
      font-family: "Fraunces";
      font-size: 1.5rem;
      color: #278575;
    }

    p {
      color: rgb(63, 158, 142)
    }

  }
  
  .orange-img {
    min-height: 87vh;
    width: 50%;
    background-image: url("../../assets/images/desktop/image-photography.jpg");
    background-repeat: no-repeat;
    background-size: 100%;
    text-align: center;
    padding: 55% 20% 20%;

    h2 {
      font-family: "Fraunces";
      font-size: 1.5rem;
      color: #1c6187;
    }

    p {
      color: #1779ae;
    }

  }
}
}

</style>