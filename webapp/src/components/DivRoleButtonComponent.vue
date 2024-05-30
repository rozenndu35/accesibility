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
    class="bouton"
    @click="click"
    @keydown="handleKeyDown"
    @keyup="handleKeyUp"
    @mousedown="handleDown"
    @mouseup="handleUp"
    role="button"
    tabindex="0"
  >
    <div>Je suis un div de role bouton avec un tab index</div>
  </div>
</template>
