<template>
    <section class="card-section">
        <h2>Card Section</h2>
        <div class="cards">
            <div class="card" v-for="card in cards" :key="card.id">
                <h3>{{ card.title }}</h3>
                <p>{{ card.description }}</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'CardSection',
    data() {
        return {
            cards: [
                { id: 1, title: 'Created with VUE', description: 'This website is created with VUE js and Vite! Also using some GSAP for animations, cuz im just like that ;)' },
                { id: 2, title: 'My first Framework', description: 'This is my first time creating a website with a framework' },
                { id: 3, title: 'By my self', description: 'Im trying to learn this by myself, because I learn better that way.' },
            ]
        };
    }
};
</script>

<style scoped>
.card-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    height: 100vh;
    background-color: #090909;

    gap: 64px
}
.card-section h2{
    font-size: 3rem;
}

.cards {
    display: flex;
    gap: 32px;
}

.card {
    border: 1px solid #ccc;
    padding: 10px;
    border-radius: 5px;
    height: 16rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 16px;

    transition: background-color .3s;
    width: 20rem;
}
.card p {
    text-align: center
}
.card:hover {
    background-color: rgba(241, 241, 241, .3);
}
</style>