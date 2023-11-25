<template>
  <MainLayout>
    <div class="container main-container">
      <div class="image-container">
        <div class="image-bg"></div>
        <g-image
          alt="About Multividas"
          src="~/assets/png/doc-logo.png"
          width="300"
          height="300"
          class="VPImage image-src"
          @load="animateImage()"
        />
      </div>
    </div>
  </MainLayout>
</template>

<script>
export default {
  metaInfo: {
    title: "About Page",
  },
  methods: {
    animateImage() {
      // image-container
      const imageContainer = document.querySelector(".image-container");
      imageContainer.classList.add("animate-image");
      // Add a class to trigger the CSS animation for image-src
      const imageSrc = document.querySelector(".image-src");
      imageSrc.classList.add("animate-image");
      // img bg
      const imageBg = document.querySelector(".image-bg");
      imageBg.classList.add("animate-image");
    },
  },
};
</script>

<style>
/* image-container */
.image-container {
  opacity: 0;
  /* Initially set opacity to 0 */
  transition: opacity 1.5s ease-in;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

/* image-bg */
.image-bg {
  opacity: 0;
  /* Initially set opacity to 0 */
  transition: opacity 1.5s ease-in;
  position: absolute;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  background-image: url("https://developers.multividas.com/images/logo-with-shadow.png");
  filter: blur(72px);
}

/* image-src */
.image-src {
  position: absolute;
  opacity: 1;
  /* Initially set opacity to 1 */
  transition: opacity 1.5s ease-in;
}

/* Keyframes for animation */
@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

/* Add the class to trigger the animation */
.animate-image {
  animation: fadeIn 1.5s ease-in;
  opacity: 1;
}
/* Extra Small Devices (Portrait Phones) */
@media only screen and (max-width: 576px) {
  .main-container {
    margin-top: 5%;
    margin-bottom: 15%;
  }

  .image-container {
    position: relative;
  }

  /* image-bg */
  .image-bg {
    position: relative;
  }

  /* image-src */
  .image-src {
    position: absolute;
    width: 200px;
    height: 200px;
  }
}

/* Small Devices (Landscape Phones) */
@media only screen and (min-width: 577px) and (max-width: 768px) {
  .main-container {
    margin-top: 25%;
    margin-bottom: 25%;
  }

  /* image-src */
  .image-src {
    position: absolute;
    width: 200px;
    height: 200px;
  }
}

/* Medium Devices (Tablets) */
@media only screen and (min-width: 769px) and (max-width: 992px) {
  .main-container {
    margin-top: 30%;
    margin-bottom: 30%;
  }
}

/* Large Devices (Desktops) */
@media only screen and (min-width: 993px) and (max-width: 1200px) {
  .main-container {
    margin-top: 25%;
    margin-bottom: 25%;
  }
}

/* Extra Large Devices (Large Desktops) */
@media only screen and (min-width: 1201px) {
  .main-container {
    margin-top: 15%;
    margin-bottom: 15%;
  }
}

/*  */
</style>
