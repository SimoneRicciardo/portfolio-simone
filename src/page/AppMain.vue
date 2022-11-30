<template>
    <div>
      <MyHeader/>
      <SectionAboutMe/>
      <SectionMyCompetenze/>
      <SectionMyContacts/>
    </div>
  </template>
  
  <script>
  import MyHeader from '@/components/MyHeader.vue';
  import SectionAboutMe from '@/components/SectionAboutMe.vue';
  import SectionMyCompetenze from '@/components/SectionMyCompetenze.vue';
  import SectionMyContacts from '@/components/SectionMyContacts.vue';

  export default {
    name: "AppMain",
    components: { MyHeader, SectionAboutMe, SectionMyCompetenze,SectionMyContacts }
}
  </script>
  
  <style scoped lang="scss">

  </style>