<script >

export default {
    name: "AppTitle",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                },
                {
                    text: "COMICS",
                    url: "#",
                },
                {
                    text: "MOVIES",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "GAMES",
                    url: "#",
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                },
                {
                    text: "VIDEOS",
                    url: "#",
                },
                {
                    text: "FANS",
                    url: "#",
                },
                {
                    text: "NEWS",
                    url: "#",
                },
                {
                    text: "SHOP",
                    url: "#",
                },
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="displayItem">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <ul class="menuItems">
                <li v-for="(link, index) in links">
                    <a :href="link.url">{{ link.text }}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped>
.container {
    background-color: white;
    height: 100px;
    display: grid;
}

.displayItem {
    width: 1400px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo img {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 80%;
}

.menuItems {
    list-style: none;
    display: flex;
    gap: 20px;
}

a {
    text-decoration: none;
    color: #666867;
}
</style>
