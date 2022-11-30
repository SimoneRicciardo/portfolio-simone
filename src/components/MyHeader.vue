<template>
    <div>
        <div class="my_container_h">
            <h1>ciao sono simone</h1>
            
            <div class="mt-5 btn_list text-end filter-btn" :class="sortList == false ? 'mb-5':''"  v-on:click="sortList = !sortList">
                <h4 class="mt-2">Vai a </h4>
                <ul class="my_list" v-show="sortList">
                    <li class="d-flex">
                        <a v-for="(link, index) in myLink" :key="index" class="px-3" :href="link.section">{{link.name}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
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
            ],
            sortList: false,
        }
    },
  }
  </script>
  
  <style scoped lang="scss">
.my_container_h{
    background-image: url(../assets/Backgorund.gif);
    background-size: cover;
    height: 100vh;
    width: 100%;
    color: white;
    .btn_list{
        position: relative;
        top: 5px;
        right: 5px;
        position: fixed;
        .my_list{
            list-style: none;
            padding: 0;
            a{
                text-decoration: none;
                color: white;
            }
        }
        .my_style_title{
            height: 100%;
        }
    }
    .filter-btn {
    border: #141913 solid 1px;
    border-radius: 5px;
    cursor: pointer;
    margin: 0 auto;
    }
}
  </style>