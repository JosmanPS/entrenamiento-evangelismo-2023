<template>
  <section class="bg-black px-2 relative overflow-hidden">
    <div class="container mx-auto">
      <div class="text-center mx-auto max-w-4xl">
        <div
          class="relative h-screen flex items-center flex-col justify-center"
        >
          <img
            class="max-w-[700px] w-full mx-auto entrenamiento-img"
            src="/img/entrenamiento.png"
            alt="Entrenamiento Evangelismo Sobrenatural"
          />
          <CTAButton class="relative mt-6" />
          <img
            class="cristian-img w-full max-w-[600px]"
            src="/img/cristian-hero.png"
            alt="Cristian Ledesma"
          />
          <img
            class="dove-img w-full max-w-[500px]"
            src="/img/dove.png"
            alt="Espíritu Santo"
          />
          <img
            class="fire-img w-full max-w-[500px]"
            src="/img/fire.png"
            alt="Fuego"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.entrenamiento-img {
  position: relative;
  z-index: 2;
}

.cristian-img {
  position: absolute;
  right: -200px;
  bottom: 0px;
  opacity: 80%;
  width: 500px;
  height: auto;
  z-index: 1;
}

.dove-img {
    position: absolute;
    right: 0px;
    top: 30px;
    width: 450px;
    height: auto;
}

.fire-img {
    position: absolute;
    left: -300px;
    bottom: -100px;
    width: 350px;
    height: auto;
}
</style>