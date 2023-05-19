<script >

export default {
    name: "AppFooterFollow",
    data() {
        return {
            socials: [
                "img/footer-facebook.png",
                "img/footer-twitter.png",
                "img/footer-youtube.png",
                "img/footer-pinterest.png",
                "img/footer-periscope.png"
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="containerFollow">
            <div class="containerItems">
                <button class="btnFooter">SIGN-UP NOW!</button>
                <ul class="socialItems">
                    <h3 class="followUs">FOLLOW US</h3>
                    <li v-for="social in socials" class="socialItemsFollow">
                        <img :src="social" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    display: grid;
    background-color: #303030;
    height: 200px;
}

.containerFollow {
    background-color: #303030;
    margin: 0 auto;
    width: 1400px;
    display: grid;
    position: sticky;
    z-index: 999999;
}

.containerItems {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.btnFooter {
    height: 50px;
    width: 150px;
    border: 1px solid #0282F9;
    background-color: #303030;
    color: white;
    cursor: pointer;
}

.followUs {
    color: #0282F9;
}

.socialItems {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
}
</style>