<script setup lang="ts"></script>

<template>
  <main>
    <div class="row justify-content-center m-0 p-0 mt-5">
      <div class="col-md-8">
        <div class="card shadow">
          <div class="card-body">
            <h1 class="card-title text-center mb-4">Contáctanos</h1>
            <form>
              <div class="mb-3">
                <label for="nombre" class="form-label">Nombre y apellido</label>
                <input
                  type="text"
                  class="form-control"
                  id="nombre"
                  placeholder="Nombre y apellido"
                />
              </div>
              <div class="mb-3">
                <label for="email" class="form-label">Correo electrónico</label>
                <input
                  type="email"
                  class="form-control"
                  id="email"
                  placeholder="name@example.com"
                />
              </div>
              <div class="mb-3">
                <label for="telefono" class="form-label">Teléfono</label>
                <input type="number" class="form-control" id="telefono" placeholder="Teléfono" />
              </div>
              <div class="mb-3">
                <label for="mensaje" class="form-label">Mensaje</label>
                <textarea
                  class="form-control"
                  id="mensaje"
                  rows="3"
                  placeholder="Mensaje"
                ></textarea>
              </div>
              <div class="text-center">
                <button type="button" class="btn btn-primary">Enviar datos</button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
