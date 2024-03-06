<template>
    <header class="bg-gray-800 text-white py-4 px-6">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="text-2xl font-bold">YB</h1>
            <nav>
                <ul class="flex space-x-4">
                    <li><RouterLink to="/home">Home</RouterLink></li>
                    <li><RouterLink to="/index">Basket</RouterLink></li>
                    <li><RouterLink to="/contact">Contact</RouterLink></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
import { RouterLink } from 'vue-router';

export default {
    name: 'Header',
    components: {
        RouterLink
    }
}
</script>
