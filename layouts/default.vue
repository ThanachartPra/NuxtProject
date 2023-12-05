<template>
    <div>
        <header>
            <nav>
                <h1 class="logo">Nuxt Sample</h1>
                <NuxtLink to="/">Home</NuxtLink>
                <NuxtLink to="/contact_us">Contact us</NuxtLink>
            </nav>
        </header>
        <div>
            <slot />
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
nav {
    margin: 10px auto;
    padding: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #333;
    border-radius: 10px;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 12px;
    font-size: 18px;
    pad: 10px;
}

nav a:hover {
    color: greenyellow;
}

.logo {
    margin-right: auto;
    padding-left: 10px;
    color: white;
}
</style>