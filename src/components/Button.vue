<template>
  <button 
    @click="onClick()" 
    color='green' 
    :style="{ background: color }" 
    class="btn">{{ text }}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
      onClick(){
          this.$emit('btn-click')
      },
  }
};
</script>