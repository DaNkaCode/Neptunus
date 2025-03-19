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
    <NavBtn
      btn-text="File"
      fir-text="New File"
      sec-text="Open File"
      th-text="New Folder"
      four-text="Open Folder"
      fif-text="Save"
    />
    <NavBtn
      btn-text="Info"
      fir-text="Github"
      sec-text="Telegram"
      th-text="Docs"
      four-text="History"
      fif-text="Support"
    />
    <NavBtn
      btn-text="Edit"
      fir-text="Undo"
      sec-text="Redo"
      th-text="Settings"
      four-text="Plugins"
      fif-text="Select All"
    />
    <NavBtn
      btn-text="Run"
      fir-text="Run Code"
      sec-text="Run Settings"
      th-text="Error checking"
      four-text="Plugins"
      fif-text="Modules"
    />
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
