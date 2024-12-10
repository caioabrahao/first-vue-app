<template>
    <section class="hero-section">
        <div class="hero-text">
        <h1>Trying to learn VUE</h1>
        <p>This is my first VUE application!</p>
        </div>
        
    </section>
</template>

<script>
export default {
    name: 'HeroSection',
    data() {
        return {
            message: 'Hello, Vue!'
        };
    },
    methods: {
        greet() {
            console.log(this.message);
        }
    }
};
</script>

<style scoped>
.hero-section {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.hero-section h1{
    font-size: 5rem;
}

.hero-text{
    display: flex;
    flex-direction: column;
    align-items: center;
}
</style>