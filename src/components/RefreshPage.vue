<script>
export default {
  methods: {
    reloadPage() {
      window.location.reload();
    }
  }
}
</script>

<template>
    <button @click="reloadPage" class="border border-gray-400 rounded px-2 py-2 ml-7 mt-2.5 ">Reload</button>
  </template>
  
  
