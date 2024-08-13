<template>
    <main>
        <div class="container py-4">
            <h2>Le nostre giornate</h2>
            <div class="row">
                <div class="col-12 col-md-6 col-lg-3 mb-4" v-for="(item, index) in day" :key="index">
                    <CardComponent :image="item.src" :title="item.titolo" :description="item.descrizione" :day="item.giorno"/>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import {day} from '../data/store.js';
import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components:{
            CardComponent
        },
        data(){
            return{
                day: day
            }
        },
        mounted(){
            console.log(this.day);
        }
    }
</script>

<style lang="scss" scoped>

</style>