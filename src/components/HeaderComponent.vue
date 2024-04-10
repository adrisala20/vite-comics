<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/img/favicon.ico" alt="logo DC">
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
header {
    padding:20px;
    height: 80px;
    display: flex;
    justify-content: space-between;
    ul{
        list-style: none;
        display: flex;
        li{
            padding: 10px 15px;
            a{
                text-decoration: none;
                color: black;
                text-transform: uppercase;
            }
        }

    }
}

</style>