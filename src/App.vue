<template>
  <div>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quo pariatur
      necessitatibus cupiditate blanditiis architecto eum rerum ullam nulla,
      culpa, adipisci quaerat similique sint.<span v-if="!more">....</span>
      <span v-else>
        Veniam corrupti harum asperiores! Omnis, error quam! Cum fuga esse aut
        nesciunt? Ab eligendi minus ut, temporibus, cum, tempore provident at
        iure harum eius placeat a iste odit quos ipsum nisi pariatur voluptates.
        Vero veritatis odio cum? Eius, optio. Quo ex, quas deserunt aperiam
        provident beatae laudantium nisi obcaecati et doloremque error eos vitae
        autem itaque natus sapiente molestiae. Totam exercitationem officiis
        mollitia rem eveniet ex cupiditate.
      </span>
    </p>
    <button @click="toggleVisibility">
      Read
      <span v-show="more">Less</span>
      <span v-show="!more">More</span>
    </button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      more: false,
    };
  },
  methods: {
    toggleVisibility() {
      return (this.more = !this.more);
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
button {
  padding: 10px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  background-color: blueviolet;
  color: white;
}
</style>
