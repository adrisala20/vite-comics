<template>
    <footer>
        <div id="footer-top">
            <div class="container">
                <ul>
                    <li v-for="(item,index) in navbar" :key="index">
                        <img :src="item.img" :alt="item.title"> 
                        <p> {{ item.title}}</p>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
    
</template>

<script>
    export default {
        name:'FooterComponentTop',
        data(){
            return{
                navbar:[
                    {
                        title:'digital Comics',
                        img:'/img/buy-comics-digital-comics.png'
                    },
                    {
                        title:'dc merchandise',
                        img:'/img/buy-comics-merchandise.png'
                    },
                    {
                        title:'subscription',
                        img:'/img/buy-comics-subscriptions.png'
                    },
                    {
                        title:'come shop location',
                        img:'/img/buy-comics-shop-locator.png'
                    },
                    {
                        title:'dc power visa',
                        img:'/img/buy-dc-power-visa.svg'
                    },                   
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    #footer-top{
        background-color: #0282F9;
        
        ul{
            list-style: none;
            display: flex;
            justify-content: start;
            align-items: center;
            width: 100%;
                li{
                    padding: 20px 15px;
                    img{
                        width: 4em;
                        margin-right: 10px;
                    };
                    p{
                        display: inline;
                        text-transform: uppercase;
                        color: white;
                    }
                }

        }
    }
    

</style>