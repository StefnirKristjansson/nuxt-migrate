<script>
/**
 * Horiontal layout
 */
export default {
  created() {
    document.body.setAttribute("data-layout", "horizontal");
    document.body.setAttribute("data-topbar", "colored");
  },
  methods: {
    toggleRightSidebar() {
      document.body.classList.toggle("right-bar-enabled");
    },
    hideRightSidebar() {
      document.body.classList.remove("right-bar-enabled");
    },
  },
};
</script>

<template>
  <!-- Begin page -->
  <div id="layout-wrapper">
    <HorizontalTopbar :type="colored" :width="fluid" />
    <!-- ============================================================== -->
    <!-- Start right Content here -->
    <!-- ============================================================== -->
    <div class="main-content">
      <div class="page-content">
        <div class="container-fluid">
          <Nuxt />
        </div>
      </div>
      <Footer />
    </div>
  </div>
</template>
