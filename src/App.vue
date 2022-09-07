<template>
  <link href="https://fonts.googleapis.com/css2?family=Didact+Gothic&display=swap" rel="stylesheet">
  <link rel="icon" type="icon"  href="../src/assets/favicon.ico">
  <myHeader></myHeader>
  <mon-accueil></mon-accueil>
  <myFooter></myFooter>
</template>

<script>

import myHeader from "@/components/myHeader";
import myFooter from "@/components/myFooter";
import MonAccueil from "@/components/monAccueil";

export default {
  name: 'App',
  components: {
    MonAccueil,
    myHeader,
    myFooter
  }
}
</script>

<style>

* {
  box-sizing: border-box;
  font-family: 'Didact Gothic', sans-serif;
}

body {
  background: var(--white-creme);
  margin: 0;
  padding: 0;
}

:root {
  --vert-the: #CCD5AE;
  --vert-the-clair: #E9EDC9;
  --white-creme: #FEFAE0;
  --orange-creme: #FAEDCD;
  --brun-clair: #D4A373;
  --white: #FFFFFF;
  --black: #000000;
  --grey: #F0F0F0
}
</style>
