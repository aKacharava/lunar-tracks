<template>
  <div class="lt-button">{{ title }}</div>
</template>

<script>
export default {
  name: "Button",
  props: {
    title: String,
  },
};
</script>

<style lang="scss" scoped>
$mainColor: #ff8383;
.lt-button {
  color: $mainColor;
  padding: 5px 10px;
  width: 25rem;
  height: auto;
  border: solid 1px $mainColor;
  border-radius: 36px;
  font-size: 25px;
  cursor: pointer;
}
</style>
