<template>
  <div class="d-flex align-center justify-center" style="height: 100vh;">
    <v-img
      class="mx-auto my-6"
      max-width="500"
      src="https://upload.wikimedia.org/wikipedia/commons/8/8c/Cars_Logo_Black.svg"
    ></v-img>
    <v-sheet width="400" class="mx-auto">
      <v-form fast-fail @submit.prevent="login">
        <v-text-field
          variant="underlined"
          v-model="email"
          label="Correo"
        ></v-text-field>

        <v-text-field
          variant="underlined"
          v-model="password"
          label="Contraseña"
        ></v-text-field>
        <a href="#" class="text-body-2 font-weight-regular"
          >¿Olvidaste la contraseña?</a
        >

        <v-btn
          type="submit"
          variant="outlined"
          color="primary"
          block
          class="mt-2"
          >Ingresar</v-btn
        >
      </v-form>
      <div class="mt-2">
        <p class="text-body-2">Crea una cuenta <a href="#">Registrarse</a></p>
      </div>
    </v-sheet>
  </div>
</template>
<script>
definePageMeta({
  layout: "blank",
});
</script>
