<template>
  <div class="header-container">
    <div>
      <div>Accueil</div>
      <div>Contact</div>
    </div>
    <div>
      <a href="https://kumgab.divtec.me/carwallpaper/" target="_blank"><button class="btn-explorer">Explorer mon dernier site</button></a>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: var(--brun-clair);
  margin: 0;
  box-shadow: rgba(0, 0, 0, 0.05) 0 1px 2px 0;  top: 0;
  left: 0;
  height: 100px;
  padding: 2em;
  filter: blur(30%);
  font-size: 20px;
}

.header-container div {
  display: inline;
  color: var(--white-creme);
}

.header-container div div {
  padding: 0.5em 1em 0.5em 1em;
}

.header-container div div:hover {
  cursor: pointer;
  outline: solid var(--white-creme) 2px;
}

.header-container div:last-child {
  margin-left: 2em;
}

.btn-explorer {
  border: solid var(--white-creme) 2px;
  padding: 0.5em 1em 0.5em 1em;
  background: transparent;
  color: var(--white-creme);
  font-size: 20px;
  border-radius: 0;
  position: relative;
  overflow: hidden;
  z-index: 1;
  -webkit-transition: color 150ms ease-in-out;
  transition: color 150ms ease-in-out;
}

.btn-explorer:after {
  content: '';
  position: absolute;
  display: block;
  top: 0;
  left: 50%;
  -webkit-transform: translateX(-50%);
  transform: translateX(-50%);
  width: 0;
  height: 100%;
  background: var(--white-creme);
  z-index: -1;
  -webkit-transition: width 150ms ease-in-out;
  transition: width 150ms ease-in-out;
}
.btn-explorer:hover {
  color: var(--brun-clair);
}
.btn-explorer:hover:after {
  width: 110%;
}

</style>