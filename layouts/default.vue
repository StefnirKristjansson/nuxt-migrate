<script>
import Vertical from "./vertical";
import Horizontal from "./horizontal";

export default {
  components: {
    Vertical,
    Horizontal,
  },
  mounted() {
    document.body.classList.remove("authentication-bg");
  },
};
</script>

<template>
  <div>
    <!-- Begin page -->
    <Vertical>
      <Nuxt />
    </Vertical>
    <!-- END layout-wrapper -->
  </div>
</template>
