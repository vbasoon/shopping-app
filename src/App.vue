<template>
  <div class="wrapper">
    <Header class="header" />
    <main class="page">
      <div class="container">
        <h1>Main content</h1>
        <blog-body :blogs="blogs" />
      </div>
    </main>

    <Footer class="footer" />
  </div>
</template>
<script>
import blogBody from "./components/blog.vue";
import Header from "./components/header.vue";
import Footer from "./components/footer.vue";
export default {
  data() {
    return {
      blogs: [
        {
          id: 1,
          title: "Title1",
          text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae blanditiis laborum quia exercitationem molestias tenetur veritatis doloribus natus accusantium velit?",
        },
        {
          id: 2,
          title: "Title2",
          text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae blanditiis laborum quia exercitationem molestias tenetur veritatis doloribus natus accusantium velit?",
        },
        {
          id: 3,
          title: "Title3",
          text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae blanditiis laborum quia exercitationem molestias tenetur veritatis doloribus natus accusantium velit?",
        },
      ],
    };
  },
  components: {
    Header,
    Footer,
    blogBody,
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
