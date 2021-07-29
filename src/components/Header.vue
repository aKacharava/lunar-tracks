<template>
  <header>
    <img src='../assets/img/logos/lunar-tracks.png' alt='' />
    <div class='title-container'>
      <h1>{{ title }}</h1>
      <h3>Tuesday, 6 April</h3>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    title: String
  }
}
</script>

<style lang='scss'>
header {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-content: center;
  justify-content: space-between;
  margin-top: 37px;
  padding: 0 62px;

  img{
    max-width: 50%;
  }
  .title-container{
    text-align: end;

    h1{
      font-size: 64px;
      font-weight: 300;
      line-height: 5rem;
    }
    h3{
      font-size: 36px;
      font-weight: 300;
    }
  }
}
</style>
