<template>
  <div class="block-heading">
    <h3 class="title">{{ textTitle }}</h3>
    <ButtonOval />
  </div>
</template>

<script>
  import ButtonOval from '../buttons/ButtonOval'

  export default {
    components: {
      ButtonOval
    },
    props: {
      textTitle: {
        type: String,
        required: true
      }
    }
  }
</script>

<style>
.block-heading {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
  z-index: 30;
}

.title {
  font-weight: 700;
  font-size: var(--fz-48);
  line-height: 130%;
  text-transform: capitalize;
  font-feature-settings: "pnum" on, "lnum" on;
}
</style>