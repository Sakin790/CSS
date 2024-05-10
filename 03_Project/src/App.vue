<script setup lang="ts">
import { Button } from '@/components/ui/button';
import { Input } from '@/components/ui/input';
import { ref } from 'vue';
import { reactive } from "vue"

let value = ref('');

const handleClick = () => {
  console.log(value.value);
};


const user = reactive({
  isLoggedIn: true,
  isActive: true
});
</script>

<template>
  <div class="flex w-full h-screen justify-center max-w-sm items-center gap-1.5">
    <Input id="email" type="email" placeholder="Email" v-model="value" />
    <Button type="submit" @click="handleClick">
      Print
    </Button>
    <h3>Message is: {{ value }}</h3>
    <div v-if="user.isLoggedIn">
      <p>You r not loggedin</p>
    </div>

  </div>
</template>
