<script >

export default {
    name: "AppMain"
}
</script>

<template>
    <div class="container">
        <div class="content">
        </div>
    </div>
</template>

<style scoped>
.container {
    background-image: url("/img/jumbotron.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    height: 400px;
    display: grid;
    color: white;

}

.content {
    width: 1400px;
    margin: 0 auto;
    color: white;
    display: flex;
    align-items: center;
}

.content img {
    width: 250px;
}
</style>