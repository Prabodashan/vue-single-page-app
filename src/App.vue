<template>
  <div>
    <p>simple text</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      activePage: 0,
      pages: [
        {
          link: { text: "Home", url: "index.html" },
          pageTitle: "Home Page",
          content: "This is the home content",
        },
        {
          link: { text: "About", url: "index.html" },
          pageTitle: "About Page",
          content: "This is the about content",
        },
        {
          link: { text: "Contact", url: "index.html" },
          pageTitle: "Contact Page",
          content: "This is the contact content",
        },
      ],
    };
  },
};
</script>
