<template>
        <div class="card" >
             <img :src="image" class="card-img-top" :alt="title">
             <div class="card-body bg-black ">
                 <h5 class="card-title">{{ title }}</h5>
             </div>
        </div>
</template>

<script>
    export default {
        name:'CardComponent',
        props:['image','title','text', 'link']

    }
</script>

<style lang="scss" scoped>

.card{
    border: none;
    cursor: pointer;
    img{
        height: 250px;
    };
    h5{
        color: white;
        text-transform: uppercase;
    }
}

</style>