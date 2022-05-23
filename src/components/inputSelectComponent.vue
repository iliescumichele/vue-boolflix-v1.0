<template>
    <div>
        <select >
            <option disabled value selected>Seleziona cosa guardare</option>
            <option >Movie</option>
            <option >TV</option>
        </select> 
    </div>
</template>

<script>
export default {
    name: 'inputSelectComponent',

    data(){
        return{
            selected: '',
        }
    }
}
</script>

<style lang="scss" scoped >

</style>