<template>
  <Header />
  <router-view />
</template>

<script>
import Header from "./components/Header.vue";
export default {
  components: { Header },
  setup() {},
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root {
  --main-bg: #1e293b;
  --parts-bg: #0f172a;
  --hover-bg: #64748b;
  --input-bg: #334155;
  --info-bg: #1d4ed8;
  --warning-bg: #c2410c;
  --error-bg: #b91c1c;
  --main-color: #f1f5f9;
  --info-color: #3b82f6;
  --warning-color: #f97316;
  --error-color: #ef4444;
}
html,
body {
  min-height: 100vh;
  min-width: 100%;
  background: var(--main-bg);
}
.btn {
  cursor: pointer;
}
</style>
