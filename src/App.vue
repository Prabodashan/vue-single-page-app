<template>
  <Navbar></Navbar>
  <RouterView></RouterView>
  <!-- <PageViewer v-if="pages.length > 0" :page="pages[activePage]"></PageViewer>

  <CreatePage @page-created="pageCreated"></CreatePage> -->
</template>

<script>
import Navbar from "./components/Navbar.vue";
import PageViewer from "./components/PageViewer.vue";
import CreatePage from "./components/CreatePage.vue";

export default {
  components: {
    Navbar,
    PageViewer,
    CreatePage,
  },
  methods: {
    pageCreated(pageObj) {
      this.pages.push(pageObj);
    },
  },
};
</script>
