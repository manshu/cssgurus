<template>
<div>
    <div class="font-sans antialiased">
      <nav class="flex items-center justify-between flex-wrap bg-grey p-6">
        <div class="flex items-center flex-no-shrink text-white mr-6">
          <span class="font-semibold text-xl tracking-tight">CSS Gurus</span>
        </div>
        <div class="block sm:hidden">
          <button @click="toggle" class="flex items-center px-3 py-2 border rounded text-grey-lighter border-grey-light hover:text-white hover:border-white">
            <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
          </button>
        </div>
        <div :class="open ? 'block': 'hidden'" class="w-full flex-grow sm:flex sm:items-center sm:w-auto">
          <div class="text-sm sm:flex-grow">
            <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-grey-lighter hover:text-white mr-4">
              Home
            </a>
          </div>
          <div>
            <a href="#" class="no-underline inline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-grey hover:bg-white mt-4 sm:mt-0">Download</a>
          </div>
        </div>
      </nav>
    </div>
    <div class="flex flex-col items-center justify-center h-screen">
        <h1 class="text-grey-dark text-4xl" v-text="msg">
            Coming Soon
        </h1>
        <p class="text-grey-dark text-4xl" v-text="msg2"></p>
    </div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to CSS Gurus.',
      msg2: 'Design | Develop | Innovate',
      open: false
    }
  },
  methods: {
    toggle() {
    this.open = !this.open
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
