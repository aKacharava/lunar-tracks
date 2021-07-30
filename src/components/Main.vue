<template>
  <main>
    <div class="lt-button-container">
      <Button title="Add Task" class="selected" />
      <Button title="Search" />
    </div>
  </main>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "Main",
  components: {
    Button,
  },
};
</script>

<style lang="scss" scoped>
$mainColor: #ff8383;
$secondColor: #ffffff;
main {
  padding: 0 62px;
  margin-top: 85px;

  .lt-button-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  .selected {
    background-color: $mainColor;
    color: $secondColor;
  }
}
</style>
