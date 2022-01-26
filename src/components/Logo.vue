<template>
    <div class="logo">
        <h1>Logo</h1>
    </div>
</template>
<script>
export default {
}
</script>
<style lang="css" scoped>
    .logo > h1{
        font-size: 50px;
        padding-top: 30px;
        padding-bottom: 30px;
        color: whitesmoke;
    }
/*----------------*/
/*      Media     */
/*----------------*/
@media (max-width: 700px) {
    .logo > h1{
        margin-top: 5px;
        margin-left: -30px;
        font-size: 50px;
    }
}
</style>