<template>
  <div class="place">
    <img :src=place.img width="235" height="300"/>
    <h2>{{place.name}}</h2>
    <p>{{place.desc}}</p>
  </div>
</template>

<script>
export default {
  props: ['place']
};
</script>

<style lang="scss" scoped>
.place {
  display: flex;
  flex-direction: column;
  width: 280px;
  height: 320px;
  justify-content: center;
  background: white;
  border: 1px solid #ddd;
  padding: 20px 20px;
  margin: 10px;

  h2 {
    margin: 0;
    text-align: center;
  }

  img {
    margin: 10px;
    align-self: center;
  }
}
</style>
