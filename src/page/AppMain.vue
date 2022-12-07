<template>
    <div class="my_style">
      <MyHero/>
      <SectionAboutMe/>
      <SectionMyCompetenze/>
      <SectionMyContacts/>
    </div>
  </template>
  
  <script>
  import MyHero from '@/components/MyHero.vue';
  import SectionAboutMe from '@/components/SectionAboutMe.vue';
  import SectionMyCompetenze from '@/components/SectionMyCompetenze.vue';
  import SectionMyContacts from '@/components/SectionMyContacts.vue';

  export default {
    name: "AppMain",
    components: {SectionAboutMe, SectionMyCompetenze, SectionMyContacts, MyHero }
}
  </script>
  
  <style scoped lang="scss">
.my_style{
    margin-left: 120px;
  }
  </style>