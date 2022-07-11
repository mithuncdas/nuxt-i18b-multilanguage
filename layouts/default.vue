<template>
    <div>
       <div class="container">
         <Header/>
        <Nuxt  class="mb-4" style="height:75vh"/>
        <!-- <Footer/> -->
       </div>
    </div>
</template>
<script>
export default {
    name:'DefaultLayout',
    head () {
        return this.$nuxtI18nHead()
    }
}
</script>
<style lang="css" scoped>
</style>