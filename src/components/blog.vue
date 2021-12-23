<template>
  <div blog__container>
    <h2>{{ headling }}</h2>
    <ul class="blog-item">
      <li class="blog-item__blog blog" v-for="blog in blogs">
        <span class="blog__id">{{ blog.id }}.</span>
        <span class="blog__title">{{ blog.title }}</span
        ><br />
        <span class="blog__text">{{ blog.text }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ["blogs"],
  headling: "blog-body",
};
</script>

<style lang="scss">
.blog-item {
  padding: 20px;
  text-align: left;

  .blog {
    font-weight: bold;
    list-style-type: none;
    margin-bottom: 20px;
    &__title {
      margin-left: 10px;
    }
  }
}
</style>
