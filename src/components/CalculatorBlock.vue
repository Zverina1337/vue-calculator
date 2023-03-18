<template>
  <div class="calculator-block">
    <output-block/>
    <input-block/>
  </div>
</template>

<script>
import OutputBlock from '@/components/OutputBlock.vue'
import InputBlock from '@/components/InputBlock.vue'

export default {
  name: 'CalculatorComponent',
  components: {
    OutputBlock,
    InputBlock
  }
}
</script>

<style lang="scss" scoped>
.calculator-block {
  display: flex;
  align-items: center;
  flex-direction: column;
  width: 20%;
  height: 50%;
  background-color: #D7D7D7FC;
}
</style>
