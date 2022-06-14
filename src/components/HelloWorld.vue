<template>
  <div class="hello">
    <h1>AARON HOPE</h1>
    <h4>Front End Web Developer</h4>
    <div id="welcome">
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Esse, repudiandae tenetur facere aspernatur voluptatibus totam sapiente corporis excepturi obcaecati autem molestiae. Voluptate corporis omnis atque tempore nostrum nihil officia aut magni nesciunt iusto? Officia, possimus?</p>
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repellat sunt excepturi id in quasi hic, nesciunt distinctio pariatur eveniet ipsum consequatur a fugit obcaecati, recusandae omnis aliquid, dignissimos at. Asperiores tempora perspiciatis debitis animi et cum alias assumenda laborum reiciendis!</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-size: 2rem;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

@media(min-width:600px) {
  #welcome {
    text-align: left;
  }
}
</style>
