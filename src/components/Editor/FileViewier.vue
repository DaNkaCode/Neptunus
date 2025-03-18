<template>
  <h2>{{ foldName }}</h2>
</template>

<script>
export default {
  name: "FileViewier",
  props: {
    foldName: String,
  },
};
</script>
