
<script setup>
  // Import du composant SabreLaser
  import SabreLaser from '@/components/SabreLaser.vue'
  // Import du magasin des sabres
  import {useSabresStore} from '@/stores/sabres'
  // Création d'une instance du magasin des sabres pour le composant
  const storeSabres = useSabresStore()
  // Récupération des données des sabres triés par ordre alphabétique
  const sabresListe = storeSabres.getSabresAZ
</script>


<template>
  <main class="page-accueil">
    <h1>Découvrez nos sabres <strong>LASER</strong></h1>

    <div class="sabres">
      <SabreLaser v-for="sabre in sabresListe" :key="sabre.id" :sabre="sabre" />
    </div>
  </main>
</template>

<style scoped>
/********** STYLE PAGE ACCUEIL *********/
.page-accueil .sabres {
  display: flex;
  flex-wrap: wrap;
  gap: 1.25rem;
  align-content: space-evenly;
  justify-content: center;
  padding: 0;
}
</style>