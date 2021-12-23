<template>
  <div class="wrapper">
    <Header class="header" />
    <main class="page">
      <div class="container">
        <h1>Main content</h1>
        <Shopping-list />
      </div>
    </main>

    <Footer class="footer" />
  </div>
</template>
<script>
import Header from "./components/header.vue";
import Footer from "./components/footer.vue";
import ShoppingList from "./components/shopping-list.vue";
export default {
  data() {
    return {};
  },
  components: {
    Header,
    Footer,
    ShoppingList,
  },
};
</script>
<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  text-align: center;
  color: #2c3e50;
}

.wrapper {
  display: flex;
  flex-direction: column;
}

.header {
  width: 100%;
  padding: 10px;
  background: #2c3e50;
}

main {
  .container {
    max-width: 1440px;
    width: 100%;
    height: 88vh;
    padding: 0 10px;
    margin: 0 auto;
    border: 2px solid red;
    h1 {
      margin-top: 20px;
      color: red;
    }
  }
}
</style>
