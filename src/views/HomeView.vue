<script setup>
import CardCmp from '../components/CardCmp.vue'
</script>

<script>
var dataList = [
  {
    imgSrc: 'src/assets/dummyImage.jpeg',
    text: "Some quick example text to build on the card title and make up the bulk of the card's content.",
    title: 'asdCard title',
    href: 'asd',
    id: '1'
  },
  {
    text: "Some quick example text to build on the card title and make up the bulk of the card's content.",
    title: 'asdCard title',
    href: 'asd',
    id: '2'
  },
  {
    imgSrc: 'src/assets/dummyImage.jpeg',
    text: "Some quick example text to build on the card title and make up the bulk of the card's content.",
    id: '3'
  },
  {
    imgSrc: 'src/assets/dummyImage.jpeg',
    title: 'asdCard title',
    id: '4'
  }
]
</script>

<template>
  <main>
    <div class="container text-center">
      <div class="row">
        <div class="col" :key="data.id" v-for="data of dataList">
          <CardCmp :data="data"></CardCmp>
        </div>
      </div>
    </div>
  </main>
</template>
