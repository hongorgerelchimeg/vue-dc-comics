<template>
  <header>
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.herf">{{link.text}}</a>
            </li>
       
        </ul>
  </header>
</template>

<script>
export default {
name: 'mainHeader',
data () {
    return {
        links: [
            {
                text: 'characters',
                herf: "#" 
            },
             {
                text: 'comics',
                herf: "#" 
            },
             {
                text: 'movies',
                herf: "#" 
            },
             {
                text: 'tv',
                herf: "#" 
            },
             {
                text: 'games',
                herf: "#" 
            },
             {
                text: 'collectibles',
                herf: "#" 
            },
             {
                text: 'videos',
                herf: "#" 
            },
             {
                text: 'fans',
                herf: "#" 
            },
             {
                text: 'news',
                herf: "#" 
            },
             {
                text: 'shop',
                herf: "#" 
            }
        ]
    }
}
}
</script>

<style lang="scss" scoped>
header {
    display: flex;
    align-items: center;
    justify-content: space-around;
    background-color: white;
    padding: 1rem 0;
}
li {
    display: inline-block;
    a {
        color: black;
        text-decoration: none;
        margin: 0 1rem;
    }

}
</style>>
    