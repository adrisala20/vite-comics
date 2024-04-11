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
    &:hover {
      box-shadow: 0 8px 16px 0 rgba(255, 255, 255, 0.787);
    }
    img{
        height: 15em;
    };
    h5{
        color: white;
        text-transform: uppercase;
    }
}

</style>