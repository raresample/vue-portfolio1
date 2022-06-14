<template>
  <div class="container">
    <h1>Completed Projects</h1>
      <!-- <ProjectCard id="helloworld" headdy="Goon Squad" title="Aaron Hope, at your service" body="Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta itaque adipisci, impedit cupiditate modi amet atque iure nemo quam illo." />
      <ProjectCard id="helloworld" headdy="Different Designers All Over" title="Aaron Hope, at your service" body="Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta itaque adipisci, impedit cupiditate modi amet atque iure nemo quam illo." /> -->
      <ProjectCard v-for="card in cardData" :key="card.index" :headdy="card.headdy" :title="card.title" :body="card.body" :imageUrl="'https://picsum.photos/300'" ></ProjectCard>


      <div class="card bg-light mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Light card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card bg-light mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Light card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card text-white bg-primary mb-3" >
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Primary card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card bg-secondary mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Secondary card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card text-white bg-success mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Success card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card text-white bg-danger mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Danger card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card text-white bg-warning mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Warning card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card text-white bg-info mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Info card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card bg-light mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Light card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>
      <div class="card text-white bg-dark mb-3">
        <div class="card-header">Header</div>
        <div class="card-body">
          <h4 class="card-title">Dark card title</h4>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        </div>
      </div>    
  </div>
</template>

<script>
// @ is an alias to /src
import ProjectCard from '@/components/ProjectCard.vue'

export default {
  name: 'HomeView',
  components: {
    ProjectCard
  },
  data() {
    return {
      cardData: [
        {index: 0, headdy: 'Different Designers All Over', title: 'Aaron Hope, at your service', body:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta itaque adipisci, impedit cupiditate modi amet atque iure nemo quam illo.'},
        {index: 1, headdy: 'Supply and Demand', title: 'Aaron Hope, at your service', body:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta itaque adipisci, impedit cupiditate modi amet atque iure nemo quam illo.'},
        {index: 2, headdy: 'Shifting the Culture', title: 'Aaron Hope, at your service', body:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque consectetur mollitia.'}
      ],
    }
  }
}
</script>

<style scoped>

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