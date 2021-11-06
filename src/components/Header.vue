<template>
  <div id="header">
    <div class="wrapper">
      <span @click="toggleSidebar()" class="menuBtn btn material-icons"
        >menu</span
      >
    </div>
  </div>
</template>

<script>
export default {
  setup(props, { emit }) {
    const toggleSidebar = () => {
      emit("toggleSidebar");
    };

    return { toggleSidebar };
  },
};
</script>

<style lang="scss" scoped>
#header {
  position: absolute;
  display: flex;
  align-items: center;
  min-height: 60px;
  min-width: 100%;
  background: var(--parts-bg);

  .menuBtn {
    margin-left: 10px;
    padding: 5px;
    color: var(--main-color);
    border-radius: 50%;
    &:hover {
      background: var(--hover-bg);
    }
  }
}
</style>