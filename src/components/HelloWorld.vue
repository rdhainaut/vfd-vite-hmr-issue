<script lang="ts">
import { Component, Prop, Vue } from 'vue-facing-decorator/dist/index-return-cons' // HMR doesn't work with this
//import { Component, Prop, Vue } from 'vue-facing-decorator' // HMR work with this

@Component
export default class HelloWorld extends Vue {
  @Prop() msg!: string
}
</script>

<template>
  <div>
    <h1>{{ msg }}</h1>
    <div>
      <!-- Edit this lorem ipsum content then save to see HRM in live (it should update the view but ... it doesn't) -->
      Lorem ipsum dolor sit amet consectetur adipisicing elit. 11
    </div>
    <h3>
      You’ve successfully created a project with
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>.
    </h3>
  </div>
</template>