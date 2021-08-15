<template>
    <NuxtLink class="link" :to="`products/${info.id}`">
        <b-card
            bg-variant="light"
            :title="info.title"
            :img-src="require(`@/assets/images/${info.image}`)"
            :img-alt="info.title"
            img-top
        >
            <b-card-text>
                {{ info.snippet }}
            </b-card-text>
        </b-card>
    </NuxtLink>
</template>

<script>
export default {
    props: ['info'],

}
</script>

<style lang="scss" scoped>
.card{
    border-radius: 5px;
    box-shadow: 0 5px 5px rgba(0, 0, 0, 0.2); 
    font-size: 0.8rem;
    height: 100%;
}

.link{
    width: 33%;
    color: #111;
    text-decoration: none; 
    
    &:hover{
        color: #590004;
    }
}

img{
    max-height: 150px;
    object-fit: cover;
}

h4{
    font-size: 1rem;
}
</style>