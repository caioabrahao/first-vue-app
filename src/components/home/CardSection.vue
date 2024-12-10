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
                { id: 1, title: 'Card 1', description: 'Description for card 1' },
                { id: 2, title: 'Card 2', description: 'Description for card 2' },
                { id: 3, title: 'Card 3', description: 'Description for card 3' },
            ]
        };
    }
};
</script>

<style scoped>
.card-section {
    display: flex;
    align-items: center;
    justify-content: center;

    height: 100vh;
    background-color: #090909;
}

.cards {
    display: flex;
    gap: 20px;
}

.card {
    border: 1px solid #ccc;
    padding: 10px;
    border-radius: 5px;
}
</style>