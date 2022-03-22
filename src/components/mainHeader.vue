<template>
  <header>
      <div class="container">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.herf">{{link.text}}</a>
            </li>
    
        </ul>
      </div>
      
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
@import "../assets/styles/main";
header .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: $mainBgHeader;
    padding: 1rem 0;
    img {
        max-height: 4rem;
    }
    ul {
        margin: 0 -1rem;
    }
}
li {
    display: inline-block;
    a {
        color: $textColor;
        text-decoration: none;
        margin: 0 1rem;
        text-transform: uppercase;
        &:hover {
            color: $mainColor;
        }
    }

}
</style>
    