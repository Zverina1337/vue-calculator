<template>
  <div class="input-block">
    <div class="input-block__content">
      <calculator-number v-for='num in 9' :number="num" :key="num + Date.now()"/>
    </div>
  </div>
</template>

<script>
import CalculatorNumber from '@/components/ui-kit/CalculatorNumber.vue'

export default {
  name: 'InputBlock',
  components: {
    CalculatorNumber
  }
}
</script>

<style lang="scss" scoped>
.input-block {
  width: 100%;
  height: 60%;
  background: gray;
  border-top-left-radius: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;

  &__content {
    display: grid;
    width: 70%;
    height: 70%;
    background: #000;
    position: absolute;
    left: 0;
  }
}
</style>
