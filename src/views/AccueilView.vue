<script setup>

</script>

<template>
  <main class="page-accueil">
    <h1>Découvrez nos sabres <strong>LASER</strong></h1>

    <div class="sabres">
      <div class="sabre">
        <router-link to="/sabre/1">
          <figure>
            <img src="/img/sl-cal.jpg" alt="Sabre laser Cal Kestis">
            <figcaption>
              <h2>Sabre laser Cal Kestis</h2>
              <div class="prix">349 CHF</div>
            </figcaption>
          </figure>
        </router-link>
      </div>
      <div class="sabre rupture">
        <router-link to="/sabre/1">
          <figure>
            <img src="/img/sl-cal.jpg" alt="Sabre laser Cal Kestis">
            <figcaption>
              <p>Noooon, les stocks sont vides !</p>
              <h2>Sabre laser Cal Kestis</h2>
              <div class="prix">349 CHF</div>
            </figcaption>
          </figure>
        </router-link>
      </div>
    </div>
  </main>
</template>

<style scoped>

</style>