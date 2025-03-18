<template>
  <h2
    :style="{
      fontFamily: 'Goldman',
      color: '#493DCB',
      fontWeight: '700',
      fontSize: '25px',
    }"
  >
    Neptunus
  </h2>
  <img :style="{ height: '70px' }" src="../assets/img/Logo.svg" alt="logo" />
</template>

<script>
export default {
  name: "LogoComp",
};
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Goldman:regular,700);
</style>
