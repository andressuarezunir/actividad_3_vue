<script setup lang="ts">
import { RouterLink } from 'vue-router'

const title = 'Barrio Getsemaní'
const description =
  ' Getsemaní es un barrio con una historia contundente que siempre ha estado ligada a los movimientos de protesta y revolución. En sus orígenes fue una isla a las afueras de la ciudad amurallada separada de la ciudad, y en tiempos coloniales fue el barrio donde vivieron muchos de los esclavos que llegaron desde África a Colombia para asentarse en el puerto de Cartagena.'
const startBtnText = 'Iniciar'
const contactBtnText = 'Conocer más'
</script>

<template>
  <header class="bg-dark py-5">
    <div class="container px-5">
      <div class="row gx-5 align-items-center justify-content-center">
        <div class="col-lg-8 col-xl-7 col-xxl-6">
          <div class="my-5 text-center text-xl-start">
            <h1 class="display-5 fw-bolder text-white mb-2">{{ title }}</h1>
            <p class="lead fw-normal text-white-50 mb-4">
              {{ description }}
            </p>
            <div class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xl-start">
              <RouterLink class="btn btn-primary btn-lg px-4 me-sm-3" to="/">{{
                startBtnText
              }}</RouterLink>
              <RouterLink class="btn btn-outline-light btn-lg px-4" to="/form">{{
                contactBtnText
              }}</RouterLink>
            </div>
          </div>
        </div>
        <div class="col-xl-5 col-xxl-6 d-none d-xl-block text-center">
          <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-indicators">
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="0"
                class="active"
                aria-current="true"
                aria-label="Slide 1"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="1"
                aria-label="Slide 2"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="2"
                aria-label="Slide 3"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="3"
                aria-label="Slide 4"
              ></button>
            </div>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="../assets/img/f1.jpg" class="d-block w-100 rounded-3 my-5" alt="..." />
              </div>
              <div class="carousel-item">
                <img src="../assets/img/f2.jpg" class="d-block w-100 rounded-3 my-5" alt="..." />
              </div>
              <div class="carousel-item">
                <img src="../assets/img/f3.jpg" class="d-block w-100 rounded-3 my-5" alt="..." />
              </div>
              <div class="carousel-item">
                <img src="../assets/img/f4.jpg" class="d-block w-100 rounded-3 my-5" alt="..." />
              </div>
            </div>
            <button
              class="carousel-control-prev"
              type="button"
              data-bs-target="#carouselExampleIndicators"
              data-bs-slide="prev"
            >
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button
              class="carousel-control-next"
              type="button"
              data-bs-target="#carouselExampleIndicators"
              data-bs-slide="next"
            >
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>
