<template>
  <button @click="handleClick">
    {{ label }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    label: {
      type: String,
      required: true
    }
  },
  data: () => ({
    clicked: false,
    show: true,
  }),
  methods: {
    handleClick () {
      this.clicked = true
      this.show = false
    }
  }
}
</script>
