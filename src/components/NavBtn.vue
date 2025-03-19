<template>
  <div class="btn-main">
    <button @click="enableList" class="navBtn">{{ btnText }}</button>
    <ul v-if="isOpen" class="list-menu">
      <li>
        <a href="https://github.com/DaNkaCode/Neptunus"
          >{{ firText }}
          <img
            v-if="firText == 'Github'"
            src="../assets/img/GithubFill.svg"
            alt=""
          />
          <img
            :style="{ width: '24px' }"
            v-else-if="firText == 'New File'"
            src="../assets/img/FileAddFilled.svg"
            alt=""
          />
        </a>
      </li>
      <li>
        <a href=""
          >{{ secText }}
          <img
            v-if="secText == 'Telegram'"
            src="../assets/img/TelegramFill.svg"
            alt=""
        /></a>
      </li>
      <hr />
      <li>
        <a href=""
          >{{ thText }}
          <img
            :style="{ width: '24px' }"
            v-if="thText == 'New Folder'"
            src="../assets/img/FolderAddFilled.svg"
            alt=""
        /></a>
      </li>
      <li>
        <a href="">{{ fourText }}</a>
      </li>
      <hr />
      <li>
        <a href=""
          >{{ fifText }}
          <img
            :style="{ width: '24px' }"
            v-if="fifText == 'Save'"
            src="../assets/img/Save.svg"
            alt=""
        /></a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "NavBtn",
  props: {
    btnText: String,
    firText: String,
    secText: String,
    thText: String,
    fourText: String,
    fifText: String,
  },
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    enableList() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Montserrat:100,200,300,regular,500,600,700,800,900,100italic,200italic,300italic,italic,500italic,600italic,700italic,800italic,900italic);

.navBtn {
  width: 130px;
  height: 50px;

  border-radius: 15px;

  background-color: #04040c;
  color: white;

  font-size: 20px;
  font-family: "Montserrat", sans-serif;
  font-weight: 700;

  box-shadow: 2px 2px 7.6px #421e71, -2px -2px 7.6px #3f33c1;
  border: none;

  transition: background-color 0.2s ease-in-out;
}

.navBtn:hover {
  background-color: #1b1b35;
}

.navBtn:active {
  background-color: #2d2d5b;
}

.btn-main {
  position: relative;
  display: inline-block;
}

.list-menu {
  position: absolute;
  top: 100%;
  left: 0;

  width: 130px;

  background-color: #04040c;
  color: white;
  box-shadow: 2px 2px 7.6px #421e71, -2px -2px 7.6px #3f33c1;

  list-style: none;

  padding: 0;
  margin: 0;

  border-radius: 10px;
}

a {
  font-family: "Montserrat", sans-serif;

  color: rgb(200, 200, 200);
  text-decoration: none;
}

a:hover {
  color: white;
  text-shadow: 0 0 3px white;
}

li {
  padding-block: 7px;
  position: relative;
}

li:hover {
  background-color: #1b1b35;
  border-radius: 10px;
}

li > a > img {
  position: absolute;
  top: 3px;
}
</style>
