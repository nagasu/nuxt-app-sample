<template>
  <section class="container">
    <div>
      <h1 class="title">
        /users/1
      </h1>
      <h2>
        {{ name }}
      </h2>
      <nuxt-link to="/users">go to users/index</nuxt-link>
    </div>
  </section>
</template>

<script>
export default {
  validate({ params }) {
    // 数値でなければならない
    return /^\d+$/.test(params.id)
  },
  asyncData(context) {
    return {
      name: 'Nagasu!!'
    }
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
