<template>
  <div>
    <div class="panel">
      <div class="panel-body">
        <h2 v-text="title"></h2>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'BaseContent',
    props: { title: String },
  }
</script>

<style>
</style>