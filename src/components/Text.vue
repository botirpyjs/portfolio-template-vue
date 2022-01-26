<template>
    <div class="text">
        <h2>{{ hello }}</h2>
        <h4>{{ matn }}</h4>
    </div>
</template>
<script>
export default {
    data() {
        return {
            hello: "Hello I'm Botir Akhmedov",
            matn: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem officia quia minima saepe doloribus fugiat unde. Quidem ea reprehenderit soluta eius atque repudiandae cupiditate cum illo earum, vitae voluptatum. Esse, porro voluptatum, libero consequuntur enim autem quasi deleniti veniam delectus incidunt totam dolorum ex placeat illum, itaque laudantium eius. Odit voluptatem aspernatur, quos beatae dolorem hic minima aliquam laudantium corporis quam doloremque tenetur vel asperiores dolore exercitationem eligendi esse eveniet!",
        }
    },
}
</script>
<style scoped>
.text{
    background-color: #00000044;
    text-align: center;
    padding: 10px;
    margin-top: 80px;
    margin-left: 200px !important;
    margin-right: 200px !important;
    color: white;
}
.text > h2{
    font-family: monospace;
    font-weight: 900;
    font-size: 40px;
    padding-bottom: 15px;
}
.text > h4 {
    font-size: 18px;
    font-weight: 500;
}
@media (max-width: 700px) {
    .text{
        margin-top: 0px;
        margin-left: 15px !important;
        margin-right: 15px !important;
    }
    .text > h2{
        font-size: 30px;
    }
    .text > h4{
        font-size: 16.5px;
    }
}
</style>