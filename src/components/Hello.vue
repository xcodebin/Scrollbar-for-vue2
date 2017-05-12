<template>
  <Scrollbar class="my-scrollbar1" v-bind:speed=100>
    <div class="scroll-me1">
      <Scrollbar class="my-scrollbar2" v-bind:speed=100>
        <div class="scroll-me2">
        </div>
      </Scrollbar>
    </div>
  </Scrollbar>
</template>

<script>
  export default {}

</script>
<style>
  body{
    background-color: aqua;
  }
  .my-scrollbar1 {
    width: 300px;
    max-width: 300px;
    max-height: 300px;
  }

  .scroll-me1 {
    min-width: 500px;
    min-height: 500px;
  }
  .my-scrollbar2 {
    width: 100px;
    max-width: 100px;
    max-height: 100px;
  }

  .scroll-me2 {
    min-width: 200px;
    min-height: 200px;
  }
</style>
