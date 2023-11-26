<template>
  <b-col class="clos">
    <div class="img_div">
      <b-img :src="imgsrc" rounded="circle" :alt="name"></b-img>
    </div>
    <p>{{ name }}</p>
  </b-col>
</template>
<script>
export default {
  props: ['name', 'imgsrc']
}
</script>
