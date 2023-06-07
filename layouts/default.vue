<template>
  <div>
    <Navbar></Navbar>
    <header>
      <!-- <h2>Intro Nuxt</h2> -->
    </header>
    <main class="container p-3 my-5 border rounded shadow">
      <slot></slot>
    </main>
    <Footer></Footer>
  </div>
</template>

<script setup>
useHead({
  titleTemplate: "%s - Intro Nuxt",
  bodyAttrs: [
    {
      class: "text-center",
    },
  ],
  link: [
    {
      rel: "stylesheet",
      href: "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css",
      integrity:
        "sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM",
      crossorigin: "anonymous",
    },
  ],
  script: [
    {
      src: "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js",
    },
  ],
});
</script>

