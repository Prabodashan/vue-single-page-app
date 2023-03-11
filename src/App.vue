<template>
  <Navbar />
  <RouterView />
  <!-- <PageViewer v-if="pages.length > 0" :page="pages[activePage]"></PageViewer>

  <CreatePage @page-created="pageCreated"></CreatePage> -->
</template>

<script>
import Navbar from "./components/Navbar.vue";

export default {
  components: {
    Navbar,
  },
  methods: {
    pageCreated(pageObj) {
      this.pages.push(pageObj);
    },
  },
};
</script>
