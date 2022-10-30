<template>
  <div>
    <header>
      <h1><NuxtLink to="/">{{ $route.name }} 페이지</NuxtLink></h1>
      <h1>Nuxt 연습 프로젝트</h1>
      <NuxtLink to="/">홈 페이지</NuxtLink>
    </header>
    <Nuxt />
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

</style>
