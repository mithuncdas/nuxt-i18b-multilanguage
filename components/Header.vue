<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
  
  <NuxtLink to="/" class="navbar-brand">MultiLanguage</NuxtLink>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item active">
        
        <NuxtLink :to="localePath('/')" class="nav-link">Home</NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink :to="localePath('/about')" class="nav-link">About</NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink :to="localePath('/contact')" class="nav-link">Contact</NuxtLink>
      </li>
      <li class="nav-item">
        <nuxt-link class="nav-link" :to="switchLocalePath('en')">English</nuxt-link>
        
        
      </li>
      <li>
        
        <nuxt-link class="nav-link" :to="switchLocalePath('bd')">Bangla</nuxt-link>
        
      </li>
      

    </ul> 
  </div>
</nav>
    </div>
</template>
<script>
export default {
    name:'AppHeader'
}
</script>
<style lang="css" scoped>
    
</style>