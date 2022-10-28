<template>
    <main>
        <div>
            <form>
                <label for="Egg1">
                    <img src="~/assets/digiegg.webp" alt="Digiegg">
                </label>
                <input type="radio" name="Egg1" id="Egg1" v-model="egg1" :on-change="chamaFuncao">
            </form>
        </div>
    </main>
</template>

<script setup>
const egg1 = ref("");

const chamaFuncao = () => {
    console.log(egg1);
}
</script>

<style scoped>
main {
    background-color: rgb(0, 87, 87);
    width: 100vw;
    height: 100vh;

    display: flex;
    justify-content: center;
    align-items: center;
}
</style>