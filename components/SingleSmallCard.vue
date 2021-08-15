<template>
  <b-col>
        <div class="image-wrapper">
            <b-img thumbnail fluid :src="require(`@/assets/images/${info.image}`)" :alt="info.title"></b-img>
            <NuxtLink  :to="`products/${info.id}`">
                <div class="title">              
                {{ info.title }}
                </div>
            </NuxtLink>
        </div>
  </b-col>
</template>

<script>
export default {
    props: ['info'],

}
</script>

<style lang="scss" scoped>
.image-wrapper{
    position: relative;
    margin: 10px;
    height: 90%;
    cursor: pointer;

    
    &:hover .title{
        height: 100%;
        padding: 10px;
        padding-top: 20%;
    }
}
img{
    object-fit: cover;
    height: 100%;
}

h4{
    font-size: 1rem;
}

.title{
    position: absolute;
    z-index: 2;
    bottom: 0;
    width: 100%;
    font-size: 0.7rem;
    height: 0px;
    background: rgba(0,0,0, 0.7);
    transition: all 0.6s ease;
    color: #fff;
    overflow: hidden;
    text-align: center;
}
</style>