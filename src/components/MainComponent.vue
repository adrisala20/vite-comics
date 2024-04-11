<template>
    <main >
        <div class="container">
            <div class="row">
                <div class="col-12 col-md-6 col-lg-2" v-for="(item,index) in comics" :key="index">
                    <CardComponent :image="item.thumb" :title="item.series"  />
                </div>
            </div>

        </div>
        
    </main>
</template>

<script>
import { comics } from '../components/data/store';
import CardComponent from './CardComponent.vue'

    export default {
        name:'MainComponent',
        components: {
            CardComponent,
        },
        data(){
            return{
                comics:comics
            }
        },
        mounted(){
            console.log(this.comics)
        }
    }
</script>

<style lang="scss" scoped>

main {
    background-color: black;
    padding: 30px;
    .container{
        color: white;
    }
}

</style>