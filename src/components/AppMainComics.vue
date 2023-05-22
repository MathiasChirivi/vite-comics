<script >

export default {
    name: "AppMainComics",
    data() {
        return {
            itemsComic: [
                {
                    img: "/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS",
                    url: "#"
                }, {
                    img: "/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE",
                    url: "#"
                }, {
                    img: "/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION",
                    url: "#"
                }, {
                    img: "/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR",
                    url: "#"
                }, {
                    img: "/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA",
                    url: "#"
                },

            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <ul class="itemsComic">
            <li v-for="item in itemsComic" class="itemsComicCentre">
                <img :src="item.img" alt="">
                <a :href="item.url">{{ item.text }}</a>
            </li>
        </ul>
    </div>
</template>

<style scoped>
.container {
    background-color: #0282F9;
    height: 250px;
    display: grid;
}

.itemsComic {
    width: 1300px;
    margin: 0 auto;
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
}

.itemsComicCentre {
    width: calc(100% / 5);
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
}

li img {
    width: calc(100%/5);
}

a {
    color: white;
    text-decoration: none;
}
</style>