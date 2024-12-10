<template>
    <header class="header">
        <div class="logo-wrapper">
            <p class="logo">FVA</p>
            <p class="logo-subtitle">First Vue Application</p>
        </div>
        
        <nav class="header__nav">
            <ul>
                <li>
                    <router-link to="/">Home</router-link>
                </li>
                <li>
                    <router-link to="/about">About</router-link>
                </li>
                <li>
                    <router-link to="/contact">Contact</router-link>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderNav',
    data() {
        return {
            // component data
        };
    },
    methods: {
        // component methods
    },
    computed: {
        // computed properties
    },
};
</script>

<style scoped>
    .header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 50px;
    background-color: #1f1f1f;

    position: absolute;
    width: 100vw;
    }

    .header__nav ul{
    display: flex;
    gap: 20px;
    list-style: none;
    }

    .logo{
        font-size: 2rem;
        font-weight: 800;
    }
    .logo-subtitle{
        font-size: .9rem;
        font-weight: 300;
    }
</style>