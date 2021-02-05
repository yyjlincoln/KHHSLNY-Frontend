<template>
  <div :class="styles[size]">
      <slot></slot>
  </div>
</template>

<script>
export default {
  data:()=>({
    styles: {
      "xl":"text-xl md:text-2xl lg:text-3xl",
      "title":"text-xl md:text-2xl lg:text-3xl font-extrabold",
    }
  }),
  props:{
    size: {
      required: true
    }
  }

}


</script>

<style>

</style>