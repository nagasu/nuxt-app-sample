<template>
  <div>
    {{ name }}
    <button @click="increment">Click</button>
    {{ cnt }}
  </div>
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'nuxt-property-decorator'

export default class extends Vue {
  @Prop({ type: String, required: true })
  name: string

  cnt = 0

  increment(): void {
    this.cnt++
  }
}
</script>
