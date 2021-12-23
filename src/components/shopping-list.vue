<template>
  <div class="shopping-list">
    <h2>{{ title }}</h2>
    <div class="shopping-list__container">
      <ul class="shoppin-list__box list">
        <li class="list__item"></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "Shopping List",
    };
  },
};
</script>

<style></style>
