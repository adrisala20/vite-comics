<template>
    <header class="container">
            <div class="col-2 logo">
            <img src="/img/dc-logo.png" alt="logo DC">
        </div>
            <ul>
                <li v-for="(item,index) in menu" :key="index">
                    <a :href="item.url">{{ item.name }}</a>
                </li>
            </ul>        
    </header>
</template>

<script>
    export default {
        name:'HeaderComponent',
        data(){
            return{
                menu:[
                    {
                        name:'Characters',
                        url:'#'
                    },
                    {
                        name:'Comics',
                        url:'#'
                    },
                    {
                        name:'Movies',
                        url:'#'
                    },
                    {
                        name:'tv',
                        url:'#'
                    },
                    {
                        name:'Games',
                        url:'#'
                    },
                    {
                        name:'collectibles',
                        url:'#'
                    },
                    {
                        name:'Videos',
                        url:'#'
                    },
                    {
                        name:'Fans',
                        url:'#'
                    },
                    {
                        name:'New',
                        url:'#'
                    },
                    {
                        name:'Shops',
                        url:'#'
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

header{
    img{
        width: 6em;
    }
}
header {
    padding: 20px;
    display: flex;
    justify-content: space-between;
    ul{
        list-style: none;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        li{
            padding: 10px 15px;
            a{
                text-decoration: none;
                color: black;
                border-bottom: 5px solid transparent;
                padding: 0px 5px 73px 0px;
            &:hover {
                color: $primary;
                border-bottom: 5px solid $primary;
                padding: 0px 5px 73px 0px;
                }

                }
            }
        }

    }


</style>