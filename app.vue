<template>
  <!-- <HomeWelcome/> -->
  <button @click="toggle">Toggle</button> <br> <br>
  <component :is="MyComponent"/>
  <!-- <Counter/> -->
</template>

<script setup>
  const MyComponent = shallowRef(resolveComponent("Counter"));

  function toggle(){
    MyComponent.value = resolveComponent("HomeWelcome");
  }

</script>
 