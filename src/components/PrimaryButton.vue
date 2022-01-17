<template>
    <button type="button" class="btn">Get in touch</button>
</template>


<script>
export default {
    name: 'PrimaryButton'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

button {
    background-color: $page-primary-color;
    color: white;
    text-transform: uppercase;
    padding: 5px 20px;
    font-size: 14px;
}
</style>