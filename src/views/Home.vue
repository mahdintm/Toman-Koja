<script setup>
import HomeItems from '../components/HomeItems.vue'
var data = [
  { name: 'slm', imgsrc: 'https://picsum.photos/1024/400/?image=41' },
  { name: 'slm', imgsrc: 'https://picsum.photos/1024/400/?image=41' },
  { name: 'slm', imgsrc: 'https://picsum.photos/1024/400/?image=41' },
  { name: 'slm', imgsrc: 'https://picsum.photos/1024/400/?image=41' }
]
</script>

<template>
  <b-container class="bv-example-row mb-3">
    <b-row cols="1" cols-sm="1" cols-md="2" cols-lg="3">
      <HomeItems
        v-for="item in data"
        :key="item.name"
        :name="item.name"
        :imgsrc="item.imgsrc"
      ></HomeItems>
    </b-row>
  </b-container>
</template>
<style>
.clos {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-content: center;
  align-items: center;
  flex-wrap: nowrap;
  padding: 5vh;
  margin: 1px;
  height: 20vw;
  background-color: aquamarine;
  width: 100%;
}
p {
  padding-top: 4vh;
}
.img_div {
  max-width: 250px;
  max-height: 250px;
  background-color: black;
}
img {
  width: 100%;
  height: 100%;
}
</style>
