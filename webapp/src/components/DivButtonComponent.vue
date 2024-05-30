<script setup lang="ts">
function handleKeyDown(event: KeyboardEvent) {
  console.log('down : ' + event.key)
}
function handleKeyUp(event: KeyboardEvent) {
  console.log('up : ' + event.key)
}
function click() {
  console.log('click ')
}
function handleDown() {
  console.log('down souris')
}
function handleUp() {
  console.log('up souris ')
}
</script>

<template>
  <div
    class="bouton boutinIntern"
    @click="click"
    @keydown="handleKeyDown"
    @keyup="handleKeyUp"
    @mousedown="handleDown"
    @mouseup="handleUp"
  >
    <button>
      <div>Je suis un bouton et ma div ecoute</div>
    </button>
  </div>
</template>
<style></style>
