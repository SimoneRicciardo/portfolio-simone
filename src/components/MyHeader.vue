<template>
        <nav class="my_header sticky-top">
            <img class="img-fluid" src="../assets/FotoProfiloC.jpg" alt="">
            <div class="d-flex justify-content-center align-items-center">
                <ul class="my_list">
                    <li class="d-flex flex-column">
                        <i></i>
                        <a v-for="(link, index) in myLink" :key="index" class="px-3" :href="link.section">{{link.name}}</a>
                    </li>
                </ul>
            </div>
        </nav>
  </template>
  
  <script>
  export default {
    name: 'MyHeader',
    data(){
        return{
            myLink: [
                {
                    name: 'Chi sono',
                    section: '#aboutme'
                },
                {
                    name: 'Competenze',
                    section: '#competenze'
                },
                {
                    name: 'Contatti',
                    section: '#contatti'
                },
                {
                    name: 'Home',
                    section: '#'
                }
            ]
        }
    },
  }
  </script>
  
  <style scoped lang="scss">
  .my_header{
    width: 120px;
    background: #222;
    color: #f1f1f1;
    height: 100%;
    position: fixed!important;
    z-index: 1;
    .my_list{
        list-style: none;
        padding: 0;
        a{
            text-decoration: none;
            color: black;
        }
    }
}
  </style>