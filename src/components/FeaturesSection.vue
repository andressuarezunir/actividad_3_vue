<script setup lang="ts">
const city = {
  name: 'Cartagena de Indias',
  description:
    'Cartagena es una ciudad portuaria en la costa caribeña de Colombia. Junto al mar, se encuentra la Ciudad Vieja amurallada, que se fundó en el siglo XVI, con plazas, calles de adoquines y edificios coloniales coloridos. Con un clima tropical, la ciudad también es un destino popular por sus playas. Se puede llegar en bote a la Isla de Barú, con playas de arena blanca y palmeras, y a las Islas del Rosario, famosas por sus arrecifes de coral.',
  image_alt: 'city image',
  features: [
    {
      title: 'MUSEOS',
      description:
        'Si ha visitado el Centro de Convenciones Cartagena de Indias, operado por Grupo Heroica, seguro ha sido recibido por ‘La Galerna’, un imponente mural que evoca lo abstracto y lo simbólico de la fauna colombiana y los vientos huracanas, con las características formas del destacado artista colombiano Alejandro Obregón, pintado previo a la inauguración del recinto en 1982.',
      icon: 'bi bi-collection'
    },
    {
      title: 'HOSPEDAJE',
      description:
        'Colombia ofrece vistas espectaculares, una gastronomía inigualable, una riqueza cultural y natural que no encuentras en otro lugar y gente amable que te espera con una sonrisa. La mezcla de todo esto da como resultado una serie de aventuras que debes tener antes de morir',
      icon: 'bi bi-building'
    },
    {
      title: 'RESTAURANTES',
      description:
        'La gastronomía de Cartagena es una mezcla de sabores intensos que se cultivan en sus tierras y producen sensaciones indescriptibles al combinarse con algunas aves, carnes rojas y productos de la ciénaga, los ríos y el mar. ¡Cada bocado es una fiesta en el paladar!',
      icon: 'bi bi-toggles2'
    },
    {
      title: 'COMPRAS',
      description:
        'La oferta comercial de Cartagena abarca desde las pequeñas tiendas familiares hasta los grandes centros comerciales. Sin olvidar los mercados semanales al aire libre o los de abastos donde encontrar los mejores productos de nuestra tierra',
      icon: 'bi bi-cash-coin'
    }
  ]
}
</script>

<template>
  <section class="py-5" id="features">
    <div class="container px-5 my-5">
      <div class="row gx-5">
        <div class="col-lg-4 mb-5 mb-lg-0">
          <h2 class="fw-bolder mb-0">{{ city.name }}</h2>
          <br />
          <p>
            {{ city.description }}
          </p>
          <img
            src="../assets/img/f4.jpg"
            class="d-block w-100 rounded-3"
            alt="{{city.image_alt}}"
          />
        </div>
        <div class="col-lg-8">
          <div class="row gx-5 row-cols-1 row-cols-md-2">
            <div class="col mb-5 h-100" v-for="(feature, id) in city.features" v-bind:key="id">
              <div class="feature bg-primary bg-gradient text-white rounded-3 mb-3">
                <i :class="feature.icon"></i>
              </div>
              <h2 class="h5">{{ feature.title }}</h2>
              <p class="mb-0">
                {{ feature.description }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
