<template>
  <header>
      <div class="container">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li @click="setActiveIndex(index)" v-for="(link, index) in links" :key="index" >
                <a :class="{active: index == activeIndex}" :href="link.herf">{{link.text}}</a>
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
            activeIndex: 1,
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
    },
    methods: {
        setActiveIndex (index) {
            this.activeIndex = index;
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
        margin: 0 -.8rem;
        height: 100%;
       
    }
}
li {
    display: inline-block;
    a {
        color: $textColor;
        text-decoration: none;
        margin: 0 .8rem;
        text-transform: uppercase;
        &:hover {
            color: $mainColor;
        }
    &.active {
            color: $mainColor;
            position: relative;
            
            
        
        &:after {
                position: absolute;
                bottom: -42px;
                background-color: $mainColor;
                height: 4px;
                width: 100%;
                display: block;
                content: '';
                margin: 0 .8rem;
        }
    }
    }


}
</style>
    