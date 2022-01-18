<template>
    <button type="button" class="btn btn-outline-success">Read More</button>
</template>


<script>
export default {
    name: 'SecondaryButton'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

button {
    color: white;
    border: 1px solid $page-primary-color;
    text-transform: uppercase;
    font-size: 14px;
    padding: 5px 18px;
    margin-left: 15px;

    &:hover {
        background-color: $page-primary-color;
    }
}

</style>