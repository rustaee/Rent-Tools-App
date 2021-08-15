<template>
    <div class="hero container">
        <b-row align-v="center" align-h="center">
            <!-- Text -->
            <b-col cols="7" class="text-container">
                <h1 class="header">Find your tools</h1>
                <p class="snippet">
                    Do you want to paint your house? Or renovate your garden? Or maybe you want to fix your broken table. Here you can look for the tools you need and borrow from your neighbors 
                </p>
                <b-button block pill size="lg" variant="danger" href="#" class="search-btn font-righteous">Start Looking</b-button>
            </b-col>
            <!-- Image -->
            <b-col cols="5" lg="4" offset-xl="1">
                <b-img src="~/assets/images/tools_08.jpg" fluid-grow alt="Hardware tools" class="image"></b-img>
            </b-col>
        </b-row>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.hero{
    margin-bottom: 20px;
}
.search-btn{
    background: #A50104;
    letter-spacing: 1px;

    &:hover{
        background: #590004;
    }
}

</style>