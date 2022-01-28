<template>
  <div>
      <header class="contenitore">
                <img src="../assets/img/dc-logo.png" alt="">
                <ul>
                    <li v-for="(element, index) in links" :key="index">
                        <strong><a :class="{'active': element.current}" href="#">{{element.text}}</a></strong>
                    </li>
                </ul>
      </header>
  </div>
</template>

<script>
export default {
    name: 'Header',
    data() {
      return{
        links: [
            {
                text: "CHARACTERS",
                url: "#",
                current: false,
            },
            {
                text: "COMICS",
                url: "#",
                current: true,
            },
            {
                text: "MOVIES",
                url: "#",
                current: false,
            },
            {
                text: "TV",
                url: "#",
                current: false,
            },
            {
                text: "GAMES",
                url: "#",
                current: false,
            },
            {
                text: "COLLECTIBILES",
                url: "#",
                current: false,
            },
            {
                text: "VIDEOS",
                url: "#",
                current: false,
            },
            {
                text: "FANS",
                url: "#",
                current: false,
            },
            {
                text: "NEWS",
                url: "#",
                current: false,
            },
            {
                text: "SHOP",
                url: "#",
                current: false,
            },
        ]
      }
    }
}
</script>

<style scoped>
    @import '../assets/style/partials/header.scss';
</style>