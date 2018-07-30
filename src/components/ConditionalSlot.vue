<template>
  <div>
    <slot v-if="showSlot" />
  </div>
</template>

<script>
export default {
  name: 'ConditionalSlot',
  props: {
    showSlot: {
      type: Boolean,
      required: true
    },
  },
}
</script>
