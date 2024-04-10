<template>
    <footer>
        <div class="container">
            <div class="row">
            <div class="col-xl-6 d-flex">
                <ul>
                    <li>ciao</li>
                </ul>
                <ul>
                    <li>dc</li>
                </ul>
                <ul>
                    <li>sites</li>
                </ul>
                 
            </div>
            <div class="col-xl-6"> logo</div>
            
        </div>
        </div>
       
    </footer>
</template>

<script>
    export default {
        name:'FooterComponent',
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
                        name:'Videos',
                        url:'#'
                    },
                    {
                        name:'News',
                        url:'#'
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>