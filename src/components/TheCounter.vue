<script setup lang="ts">
const props = defineProps<{
  initial: number
}>()

const { count, inc, dec } = useCounter(props.initial)
</script>

<template>
  <div>
    <button rd-r-0 btn text="xl" @click="dec()">
      -
    </button>
    <div bg="teal-950" rd-0 btn text="xl" hover="bg-teal-950" cursor="text">
      {{ count }}
    </div>
    <button rd-l-0 btn text="xl" @click="inc()">
      +
    </button>
  </div>
</template>
