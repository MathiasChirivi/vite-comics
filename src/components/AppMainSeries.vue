<script >

export default {
    name: "AppMainSeries",
    props: {
        itemsComic: Object,
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="container">
        <button class="currentSeries">CURRENT SERIES</button>
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

<style lang="scss" scoped>
$Background_color: #303030;
$Height_Container: 750px;
$width_Container: 1300px;
$display_flex: flex;
$Justify_center: center;
$Align_center: center;
$Flex_column: column;

.container {
    height: $Height_Container;
    background-color: $Background_color;
    position: relative;
}

.currentSeries {
    position: absolute;
    top: -3%;
    left: 15%;
    width: 200px;
    background-color: #0282F9;
    color: white;
    border: 1px solid #0282F9;
    height: 50px;
    font-weight: bolder;
}

.containerItems {
    width: $width_Container;
    margin: 0 auto;
    display: $display_flex;
    justify-content: $Justify_center;
    align-items: $Align_center;
    flex-direction: $Flex_column;
    ;
}

.itemsComic {
    width: $width_Container;
    padding-top: 50px;
    margin: 0 auto;
    list-style: none;
    display: $display_flex;
    flex-wrap: wrap;
    justify-content: $Justify_center;
    align-items: $Align_center;
}

.itemsComicCentre {
    height: calc(650px / 2);
    width: calc(1300px / 6);
    display: $display_flex;
    flex-direction: $Flex_column;
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