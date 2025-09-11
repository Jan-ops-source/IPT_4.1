<script setup lang="ts">
defineProps({
  title :String,
  teaser :String,
  image :String,
  NumberOfWords :Number})
</script>

<template>

      <div class="newsfeed__item">
        <div class="newsfeed__image">
          <img :src= "image" alt="">
        </div>
        <div class="newsfeed__text">
          <h2 class="newsfeed__heading">
            Lorem ipsum dolor sit amet, consetetur sadipscing elitr
          </h2>
          <p class="newsfeed__teaser">
            At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
          </p>
          <p class="newsfeed__meta">
            2 Minuten Lesezeit
          </p>
        </div>
      </div>
</template>

<style scoped>
.newsfeed__image img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.newsfeed__text {
  padding: 20px;
}

.newsfeed__item {
  display: grid;
  grid-template-columns: 200px auto;
}

.newsfeed__heading {
  font-size: 18px;
  margin: 10px 0;
}

.newsfeed__teaser {
  font-size: 15px;
  line-height: 1.25;
}

.newsfeed__meta {
  font-size: 15px;
  line-height: 1.25;
  color: rgba(255, 255, 255, .6);
}

.newsfeed__item + .newsfeed__item {
  border-top: 1px solid hsla(0,0%,100%,.05);
}
</style>