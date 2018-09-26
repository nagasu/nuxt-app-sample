<template>
  <section class="container">
    <div>
      <h1 class="title">
        /users
      </h1>
      <nuxt-link to="/users/1">go to users/1</nuxt-link>
      <nuxt-link to="/users/nagasu">go to users/nagasu</nuxt-link>
      <div>
        <nuxt-link to="/">go to top</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import Hello from '~/components/Hello.vue'

export default {
  components: {
    Hello
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
