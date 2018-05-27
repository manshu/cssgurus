<template>
    <div class="flex flex-col items-center justify-center h-screen">
        <h1 class="text-grey-dark text-4xl" v-text="msg"></h1>
        <p class="text-grey-dark text-4xl" v-text="msg2"></p>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to CSS Gurus.',
      msg2: 'Design | Develop | Innovate'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
