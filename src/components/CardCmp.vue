<script setup>
const props = defineProps({
  data: Object
})
</script>

<template>
  <div class="card" style="width: 18rem">
    <div v-if="data.imgSrc">
      <img :src="data.imgSrc" class="card-img-top" alt="..." />
    </div>

    <div class="card-body">
      <h5 v-if="data.title" class="card-title">{{ data.title }}</h5>
      <p v-if="data.text" class="card-text">
        {{ data.text }}
      </p>

      <a v-if="data.href" href="data.href" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>
</template>
