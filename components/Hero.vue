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
          <CTAButton class="relative mt-6 z-10" />
          <img
            class="cristian-img w-[500px] bottom-0 right-[-100px] md:right-[-100px] lg:right-[-200px]"
            src="/img/cristian-hero.png"
            alt="Cristian Ledesma"
          />
          <img
            class="dove-img w-[450px] right-0 top-[30px]"
            src="/img/dove.png"
            alt="Espíritu Santo"
          />
          <img
            class="fire-img w-[350px] left-[-200px] bottom-[-100px] lg:left-[-300px] md:bottom-[0px] md:left-[-100px] lg:bottom-[-100px]"
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
  opacity: 80%;
  height: auto;
  z-index: 1;
}

.dove-img {
    position: absolute;
    height: auto;
}

.fire-img {
    position: absolute;
    height: auto;
}
</style>