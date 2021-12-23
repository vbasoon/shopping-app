<template>
  <header class="header">{{ title }}</header>
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

<style lang="scss">
.header {
  width: 100%;
  padding: 10px;
  background: #2c3e50;
  color: white;
  font-size: 24px;
}
</style>
