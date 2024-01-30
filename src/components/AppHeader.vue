<script>
export default {
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <header>
    <div class="container">
      <div>
        <ul>
          <li>
            <router-link :to="{ name: 'home' }"> Home</router-link>
          </li>
          <li>
            <router-link :to="{ name: 'aboutus' }"> aboutus</router-link>
          </li>
          <li>
            <router-link :to="{ name: 'starthere' }">starthere</router-link>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/main" as *;
@use "../assets/scss/partials/variables.scss" as *;
header{
    ul{
    list-style: none;
    padding: 0;
    margin: 0;
        li{
         padding: 0;
        }
    }

}

</style>
