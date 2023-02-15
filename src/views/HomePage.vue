<template>
  <div class="home-page">
    <div class="home-page-main">
      {{ count }}

      <button
        @click="increaseCount"
        type="button">click</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increaseCount() {
      this.count += 1;
    },
  },
};
</script>

<style lang="scss">

.home-page-main {
  display: flex;
  width: 100%;
  justify-content: center;
}

</style>
