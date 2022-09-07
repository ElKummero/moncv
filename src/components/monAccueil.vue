<template>
  <div class="accueil-container">
    <div>
      <div>
        <div class="container-sections">
          <div class="selection-parcour" v-on:click="switchParcour()">Parcour</div>
          <div class="selection-passions" v-on:click="switchPassions()">Passions</div>
        </div>
        <div>
          <div class="container-parcour">
            <h2>Yo man</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam atque cum, cupiditate deleniti dolor doloribus eaque eum, expedita explicabo hic inventore, iste iusto labore nemo odio optio quis unde voluptatibus!</p>
          </div>
          <div class="container-passions">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Assumenda eum itaque labore libero maxime totam! Ab amet debitis dolores doloribus, ducimus harum modi necessitatibus odio odit officia optio soluta, ullam!</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  computed: {

  },

  methods: {

    switchParcour() {
      let parcour = document.getElementsByClassName('selection-parcour');
      let passions = document.getElementsByClassName('selection-passions');

      parcour.style.boxShadow = 'rgba(40, 40, 40, 0.2) 3px 3px 6px 0 inset, rgba(0, 0, 0, 0.2) -3px -3px 6px 1px inset';
      passions.style.boxShadow = 'rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px';
    },

    switchPassions() {
      let parcour = document.getElementsByClassName('selection-parcour');
      let passions = document.getElementsByClassName('selection-passions');

      parcour.style.boxShadow = 'rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px';
      passions.style.boxShadow = 'rgba(40, 40, 40, 0.2) 3px 3px 6px 0 inset, rgba(0, 0, 0, 0.2) -3px -3px 6px 1px inset';
    }
  }
}

</script>

<style scoped>

.accueil-container {
  padding: 2em;
  display: flex;
  width: 80%;
  height: 100%;
  background: var(--orange-creme);
  margin: auto;
}

.container-sections {
  display: flex;
  justify-content: left;
}

.container-sections div {
  font-size: 20px;
  padding: 0.5em 1em 0.5em 1em;
  background: var(--brun-clair);
  border-radius: 8px;
  color: var(--white-creme);
}

.container-sections div:hover {
  cursor: pointer;
}

.container-sections div:last-child  {
  margin-left: 1em;
}

.container-passions {
  display: none;
}

.container-passions:hover {

}

.container-parcour {
  display: block;
}

.container-parcour:hover {

}

.selection-parcour {
  box-shadow: rgba(40, 40, 40, 0.1) 3px 3px 6px 0 inset, rgba(0, 0, 0, 0.1) -3px -3px 6px 1px inset;
}

.selection-passions {
  box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
}



</style>