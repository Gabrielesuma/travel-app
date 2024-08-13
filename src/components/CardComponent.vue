<template>
    <div class="card">
        <img :src="image" class="card-img-top" :alt="title">
        <div class="card-body">
            <h3>Giorno {{ day }}</h3>
            <h5 class="card-title">{{ title }}</h5>
            <p class="card-text">{{ description }}</p>
            <a href="#" class="btn btn-primary" v-if="link">{{ link }}</a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ['image', 'title', 'description', 'day', 'link']
}
</script>

<style lang="scss" scoped></style>