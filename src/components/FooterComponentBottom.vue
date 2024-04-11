<template>
    <footer>
        <div class="container">
            <button> 
                sign-up Now!
            </button>
        </div>
        <div class="right">
            <p>follow us</p>
            <div>
                <img :src="item.img" :alt="item.title" v-for="(item,index) in navbar":key="index">
            </div>
            

        </div>
    </footer>
</template>

<script>
    export default {
        name:'FooterComponent',
        data(){
            return{
                navbar:[
                    {
                        title:'logo facebook',
                        img:'/img/footer-facebook.png'
                    },
                    {
                        title:'logo twitter',
                        img:'/img/footer-twitter.png'
                    },
                    {
                        title:'logo youtube',
                        img:'/img/footer-youtube.png'
                    },
                    {
                        title:'logo piterest',
                        img:'/img/footer-pinterest.png'
                    },
                    {
                        title:'logo-periscope',
                        img:'/img/footer-periscope.png'
                    },                   
                ]

            }
        }
    }
</script>

<style lang="scss" scoped>
footer {
    background-color: #303030;
    display: flex;
    justify-content: space-between;
    button{
        text-transform: uppercase;
        margin: 20px;
        padding: 10px;
        color: white;
        background-color: #303030;
        border-color: #0282F9;
        border-width: 2px;
    };
}
.right{
    width: 50%;
    display:flex;
    justify-content: center;
    align-items: center;
    p{
        display: inline;
        color:#0282F9;
        align-items: center
    };
    img{
        padding-left: 20px;
    }
}


</style>