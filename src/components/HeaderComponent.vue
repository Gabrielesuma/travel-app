<template>
    <header>
        <h1>My journey</h1>
        <ul>
            <li v-for="(item, index) in menu" :key="index">
                <a :href="item.url">{{ item.name }}</a>
            </li>
        </ul>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data(){
            return{
                menu:[
                    {
                        name:'Home',
                        url:'#'
                    },
                    {
                        name:'Giornate',
                        url:'#'
                    },
                    {
                        name:'Info',
                        url:'#'
                    },
                    {
                        name:'Contatti',
                        url:'#'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: lightgreen;
    h1{
        margin: 30px;
    }
}

ul {
    list-style: none;
    margin: 30px 0;
    display: flex;
    justify-content:center;

    li {
        margin: 0 20px;

        a {
            padding: 6px 10px;
            text-decoration: none;
            color: black;
        }
    }
}
</style>