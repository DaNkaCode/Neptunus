<template>
  <TextEditor />
  <FileViewier fold-name="" />
</template>

<script>
import TextEditor from "./Editor/TextEditor.vue";
import FileViewier from "./Editor/FileViewier.vue";

export default {
  name: "MainSection",
  components: {
    TextEditor,
    FileViewier,
  },
};
</script>
