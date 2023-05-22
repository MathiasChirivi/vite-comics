<script >

export default {
    name: "AppFooterImg",
    data() {
        return {
            comics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shops: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            DC: [
                "Terme of Use",
                "Privacy Policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPCS Certificates",
                "Ratings",
                "Shop Help",
                "Contact us"
            ],
            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ],
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="itemsFooter">
            <div class="left">
                <div class="containerVoce">
                    <ul class="marginTop">
                        <h3 class="marginBottom">DC COMICS</h3>
                        <li v-for="comic in comics" class="ItemsComicsVoce">
                            <a href="#">{{ comic }}</a>
                        </li>
                    </ul>
                    <ul class="marginTop">
                        <h3 class="marginBottom">SHOP</h3>
                        <li v-for="shop in shops" class="ItemsComicsVoce">
                            <a href="#">{{ shop }}</a>
                        </li>
                    </ul>
                </div>
                <div class="containerVoce">
                    <ul class="marginTop">
                        <h3 class="marginBottom">DC</h3>
                        <li v-for="DCs in DC" class="ItemsComicsVoce">
                            <a href="#">{{ DCs }}</a>
                        </li>
                    </ul>
                </div>
                <div class="containerVoce">
                    <ul class="marginTop">
                        <h3 class="marginBottom">SITES</h3>
                        <li v-for="site in sites" class="ItemsComicsVoce">
                            <a href="#"> {{ site }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="right">
                <div class="dcLogo">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>

        </div>
    </div>
</template>

<style scoped>
.container {
    background-image: url("/img/footer-bg.jpg");
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 500px;
    display: grid;
    color: white;

}

.itemsFooter {
    width: 1400px;
    margin: 0 auto;
    display: flex;
}

.left {
    width: calc(100% / 2);
    height: 500px;
    display: flex;
}

.containerVoce {
    width: calc(100% / 3);
    font-size: large;
}

.ItemsComicsVoce {
    list-style: none;
}

a {
    text-decoration: none;
    color: grey;
}

a:hover {
    color: #0282F9;
}

.marginTop {
    margin-top: 70px;
}

.marginBottom {
    margin-bottom: 20px;
}

.right {
    width: calc(100% / 2);
    height: 500px;
    position: relative;
}

.dcLogo img {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>