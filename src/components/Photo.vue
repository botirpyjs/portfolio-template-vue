<template>
<div class="photo">
    <div class="intro">
        <h2>Photo travels</h2>
        <h4>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit molestias voluptate voluptatum provident tenetur hic sapiente quibusdam neque eveniet consectetur.</h4>
    </div>
    <div class="album">
        <photo-al />
    </div>
</div>
</template>
<script>
import PhotoAl from './components/PhotoAlbum.vue'
export default {
    components: {
        PhotoAl,
    }
}
</script>
<style scoped>
.photo > .intro > h2{
    color: royalblue;
    font-size: 50px;
    padding-top: 20px;
    padding-bottom: 20px;
    text-align: center;
}
.photo > .intro > h4{
    font-size: 25px;
    text-align: center;
    padding-left: 60px !important;
    padding-right: 60px !important;
    padding-bottom: 10px;
    color: #444;
}
.photo{
    padding-bottom: 15px;
    border-bottom: crimson 2px solid;
}

@media (max-width: 700px) {
    .photo > .intro > h2{
    color: royalblue;
    font-size: 20px;
    padding-top: 5px;
    padding-bottom: 5px;
    text-align: center;
    }
    .photo > .intro > h4{
        font-size: 15px;
        text-align: center;
        padding-left: 20px !important;
        padding-right: 20px !important;
        padding-bottom: 10px;
        color: #444;
    }
    .photo{
        width: 100%;
        margin: 0 !important;
        padding-bottom: 15px;
        border-bottom: crimson 2px solid;
    }
}
</style>