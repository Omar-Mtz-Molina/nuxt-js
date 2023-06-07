<template>
  <Head>
    <Title>Post {{ id }}</Title>
  </Head>
  <h1>Bienvenido al Post # {{ id }}</h1>
</template>

<script setup>
    const { id } = useRoute().params;
    if(/^\d+$/.test(id)){
      throw createError({
        statusCode: "500",
        statusMessage: "Param Type Is Invalid"
      })
    }
    /* definePageMeta({
        validate: async (route) => {
            const nuxtApp = useNuxtApp();
            return /^\d+$/.test(route.params.id);
        }
    }) */
</script>