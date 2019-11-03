<template>
  <div class="header">
    <div class="header-title">
      <h1>Create Organization</h1>
    </div>
    <p class="header-content">
      Small or large, any team will increase productivity with HubGets.
      <br />It allows team to filter noise and focus on results.
    </p>
  </div>
</template>
<script>
export default {
  name: "HeaderDescription",
  props: {}
};
</script>
<style scoped>
.header {
  background: #00b5ef;
  height: 30vh;
}
.header-title {
  text-align: center;
  color: white;
  padding-top: 3vh;
}
.header-content {
  color: white;
}
</style>