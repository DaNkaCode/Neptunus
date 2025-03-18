<template>
  <nav
    :style="{
      display: 'flex',
      columnGap: '15px',
      alignItems: 'center',

      backgroundColor: '#04040C',

      maxWidth: '1469px',

      margin: '0 auto',

      paddingBlock: '7px',
      paddingInline: '14px',

      borderRadius: '15px',
      boxShadow: '2px 2px 7.6px #421E71, -2px -2px 7.6px #3F33C1',
    }"
  >
    <NavBtn btn-text="File" />
    <NavBtn btn-text="Info" />
    <NavBtn btn-text="Edit" />
    <NavBtn btn-text="Run" />
    <Logo />
  </nav>
</template>

<script>
import NavBtn from "./NavBtn.vue";
import Logo from "./Logo.vue";

export default {
  name: "NavBar",
  components: {
    NavBtn,
    Logo,
  },
};
</script>
