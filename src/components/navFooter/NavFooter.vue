<template>
    <div>
        <div>
            已完成 {{isComplete}} / 全部 {{all}}
        </div>
        <button v-if="isComplete > 0">清除已完成</button>
    </div>
</template>

<script>
import {defineComponent, ref} from 'vue'

export default defineComponent({
  name: 'navFooter',
  setup() {
    let isComplete = ref(1)
    let all = ref(3)
    return {
      isComplete,
      all
    } 
  },
})
</script>

<style scoped lang="scss">
    
</style>