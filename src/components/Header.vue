<template>
  <header>
    <img src='../assets/img/logos/lunar-tracks.png' alt='' />
    <div class='title-container'>
      <h1>{{ title }}</h1>
      <h3>{{ dateBuilder() }}</h3>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    title: String
  },
  methods: {
    dateBuilder () {
      const currentDate = new Date()
      const months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
      const days = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday']

      const date = currentDate.getDate()
      const day = days[currentDate.getDay()]
      const month = months[currentDate.getMonth()]
      const year = currentDate.getFullYear()

      return `${day}, ${date} ${month} ${year}`
    }
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
    height: auto;
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
