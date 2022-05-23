<template>
    <div class="header">
        <div class="logo">
            <p>logo</p>
        </div>
        <div class="components">
            <searchBarComponent />
            <inputSelectComponent />
        </div>


    </div>
</template>

<script>
import searchBarComponent from './searchBarComponent.vue'
import inputSelectComponent from './inputSelectComponent.vue'

export default {
    name: 'headerComponent',
    components: {
        searchBarComponent,
        inputSelectComponent
    }
}
</script>

<style lang="scss" scoped>
    .header{
        padding: 20px;
        height: 80px;
        opacity: 50;
        display: flex;
        align-content: center;
        justify-content: space-between;
        background-color: rgba(0, 0, 0, 0.196);

        .components{
            display: flex;
            align-content: center;
        }
    }
</style>