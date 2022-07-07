<script setup>
import {io} from 'socket.io-client';

const socket = io('http://localhost:8088');
socket.on('connect', () => {
  console.log('Server Connected');
});

</script>

<template>
  <h1>hello from index</h1>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
