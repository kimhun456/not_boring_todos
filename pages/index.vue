<script setup lang="ts">
let message = ref("message");

function onClick() {
  console.log("onClick()");
  message.value = "message is changed";
}
</script>

<template>
  <div>
    <h1>Welcome to the homepage</h1>
    <AppAlert> This is an auto-imported component </AppAlert>
    <Button @click="onClick">{{ message }}</Button>
    <Button>Button2</Button>
  </div>
</template>
