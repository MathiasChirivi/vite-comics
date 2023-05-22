<script >

export default {
    name: "AppMainSeries",
    props: [
        "itemsComic"
    ],
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="container">
        <div class="containerItems">
            <ul class="itemsComic">
                <li v-for="thumb in itemsComic" class="itemsComicCentre">
                    <img :src="thumb.thumb" alt="">
                    <div class="textThumb">{{ thumb.series }}</div>
                </li>
            </ul>
            <button class="loadSlides">LOAD MORE</button>
        </div>
    </div>
</template>

<style scoped>
.container {
    height: 750px;
    background-color: #303030;
}

.containerItems {
    width: 1300px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.itemsComic {
    width: 1300px;
    padding-top: 50px;
    margin: 0 auto;
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.itemsComicCentre {
    height: calc(650px / 2);
    width: calc(1300px / 6);
    display: flex;
    flex-direction: column;
    padding: 10px;
}

li img {
    height: 80%;
    width: 100%;
    margin-bottom: 10px;
}

.textThumb {
    color: white;
    text-transform: uppercase;
}

.loadSlides {
    margin-top: 15px;

    background-color: #0282F9;
    width: 150px;
    color: white;
    border: 0px solid white;
    height: 25px;
    cursor: pointer;

}
</style>