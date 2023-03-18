<template>
  <div class="calculator-number" @click="$emit('click')">
    {{ number }}
  </div>
</template>

<script>
export default {
  name: 'CalculatorNumber',
  props: {
    number: {
      type: Number,
      required: true,
      default: 0
    }
  }
}
</script>

<style lang="scss" scoped>
.calculator-number {
  border-radius: 20px;
  font-size: 25px;
  display: flex;
  color: white;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}
</style>
