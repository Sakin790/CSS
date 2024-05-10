<script setup lang="ts">
import { Button } from '@/components/ui/button';

function handleClick() {
  alert('You clicked the button!');
}
</script>

<template>
  <div class="w-full h-screen bg-black ">
    <Button variant="secondary" @click="handleClick">Click me</Button>
  </div>
</template>
