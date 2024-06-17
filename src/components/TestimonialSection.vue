<script setup lang="ts">
const testimonial = {
  description:
    'Cartagena, suma a sus encantos los atractivos de una intensa vida nocturna, festivales culturales y paisajes exhuberantes. Las playas de la ciudad te invitan a hacer turismo, descansar y divertirte con la refrescante brisa y las tibias aguas del mar.',
  user: {
    name: 'Tom Ato',
    city: 'Fakhouri',
    country: 'Francia'
  }
}
</script>

<template>
  <div class="py-5 bg-light">
    <div class="container px-5 my-5">
      <div class="row gx-5 justify-content-center">
        <div class="col-lg-10 col-xl-7">
          <div class="text-center">
            <div class="fs-4 mb-4 fst-italic">
              "{{ testimonial.description.split('.')[0] }}.
              <b> {{ testimonial.description.split('.')[1] }}</b
              >"
            </div>
            <div class="d-flex align-items-center justify-content-center">
              <img class="rounded-circle me-3" src="../assets/img/avatar.jpg" alt="avatar" />
              <div class="fw-bold">
                {{ testimonial.user.name }}
                <span class="fw-bold text-primary mx-1">/</span>
                {{ testimonial.user.city }} - {{ testimonial.user.country }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
