<script setup lang="ts">
import ButtonComponent from '../components/ButtonComponent.vue'
import DivButtonComponent from '../components/DivButtonComponent.vue'
import DivRoleButtonComponent from '../components/DivRoleButtonComponent.vue'
import ResultComponent from '../components/ResultComponent.vue'
</script>

<template>
  <main>
    <ButtonComponent></ButtonComponent>
    <DivButtonComponent></DivButtonComponent>
    <DivRoleButtonComponent></DivRoleButtonComponent>

    <ResultComponent></ResultComponent>
  </main>
</template>
<style lang="scss">
table {
  border-collapse: collapse;
  border: 2px solid rgb(140 140 140);
  font-family: sans-serif;
  font-size: 0.8rem;
  letter-spacing: 1px;
}

caption {
  caption-side: bottom;
  padding: 10px;
  font-weight: bold;
}

thead,
tfoot {
  background-color: rgb(228 240 245);
}

th,
td {
  border: 1px solid rgb(160 160 160);
  padding: 8px 10px;
}

td {
  text-align: center;
}

.bouton {
  position: inherit;
  justify-content: center;
  align-items: center;
  text-align: center;
  display: inline-block;
  background-color: #eee;
  color: black;
  padding: 14px 15px;
  margin: 14px 15px;
  border: none;

  &:hover,
  &:focus,
  &:focus-visible {
    outline-color: #bbb;
    color: black;
  }
  &:active {
    background-color: orange;
  }
  &:focus-visible,
  *:focus-visible {
    outline: 0.2rem solid orange;
  }

  &.boutinIntern {
    padding: 0;
  }
  button {
    background-color: transparent;
    border: 0 transparent;
    width: 100%;
    height: 100%;
    padding: 14px 15px;
  }
}
</style>
