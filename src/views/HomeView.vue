<template>
    <div class="d-flex">
 <SideNav />
  <div>
        <NavBar />
  <ContentSection />
  </div>

      
      </div>
    
  
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import ContentSection from '@/components/ContentSection.vue';
import SideNav from '@/components/SideNav.vue';

export default {
  name: 'HomeView',
  components: {
    NavBar,
    ContentSection,
    SideNav,
  }
}
</script>

<style>

</style>