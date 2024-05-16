<script>
import LeftBar from './LeftBar.vue';
import Mid from './Mid.vue';
import Right from './Right.vue';



export default {
  components: {
    LeftBar,
    Mid,
    Right
  }
}
</script>

<template>
  <div class="">
    <Right />
  </div>
  <div class="grid  grid-cols-12 h-screen w-screen ">
    <div class="col-span-4 ">
      <LeftBar />
    </div>
    <div class="col-span-8 sticky border-r-[1px] border-l-[1px] border-gray-500 ">
      <Mid />
    </div>
  </div>
</template>