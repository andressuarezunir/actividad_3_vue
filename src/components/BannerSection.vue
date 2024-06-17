<script setup lang="ts">
const text =
  'Que hermosa eres imperial Cartagena, coronada de murallas y antiguos balcones, con tu majestuosidad y señorío. Que a los turistas robas sus corazones.'
</script>

<template>
  <section class="container px-5 pt-3 pb-5">
    <aside class="bg-primary bg-gradient rounded-3 p-4 p-sm-5 mt-5">
      <div
        class="d-flex align-items-center justify-content-between flex-column flex-xl-row text-center text-xl-start"
      >
        <div class="mb-4 mb-xl-0">
          <div class="fs-3 fw-bold text-white">"{{ text }}"</div>
        </div>
      </div>
    </aside>
  </section>
</template>
