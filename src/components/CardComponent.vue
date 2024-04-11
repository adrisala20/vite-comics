<template>
        <div class="card" >
             <img :src="image" class="card-img-top" :alt="title">
             <div class="card-body">
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

</style>