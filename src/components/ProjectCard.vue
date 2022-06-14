<template>
  <!-- <div class="container"> -->
    <div class="card bg-light mb-3">
      <div class="card-header">{{ headdy }}</div>
      <div class="card-body">
        <h4 class="card-title">{{ title }}</h4>
        <img :src="imageUrl" alt="aaron hope web developer projects">
        <p class="card-text">{{ body }}</p>
      </div>
    </div>
  <!-- </div> -->
</template>

<script>
export default {
  name: 'ProjectCard',
  props: {
    index: String,
    headdy: String,
    title: String,
    body: String,
    imageUrl: String,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card {
  width: 100%;
}

.card-header {
  color: white;
  background-image: linear-gradient(
    to left, rgba(78, 217, 217, 0.761) 0%,
    rgb(128, 155, 217) 100%
  );
}

img {
  margin-bottom: .75rem;
}

div.card:hover {
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
}

/* div.card-body:hover {
  background-color: lightyellow;
} */

/* div.card-body {
  background: linear-gradient(#1095c1 0 0) calc(100% - var(--p,0%)) / var(--p,0%) no-repeat;
  transition: .25s,background-position 0s;
}
div.card-body:hover {
  --p: 100%;
  color: #fff;
} */



@media(min-width:769px) {
  .card {
    float: left;
    width: 49%;
    box-sizing: border-box;
  }
  .card:nth-of-type(odd) {
    margin-right: 1%;
  }
  .card:nth-of-type(even) {
    margin-left: 1%;
  }
}
</style>
