<template>
  <button
    :style="{
      width: '130px',
      height: '50px',
      borderRadius: '15px',
      backgroundColor: '#04040C',
      color: 'white',
      fontSize: '20px',
      boxShadow: '2px 2px 7.6px #421E71, -2px -2px 7.6px #3F33C1',
      border: 'none',
      fontFamily: 'Montserrat',
      fontWeight: '500',
    }"
  >
    {{ btnText }}
  </button>
</template>

<script>
export default {
  name: "NavBtn",
  props: {
    btnText: String,
  },
};
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Montserrat:100,200,300,regular,500,600,700,800,900,100italic,200italic,300italic,italic,500italic,600italic,700italic,800italic,900italic);
</style>
