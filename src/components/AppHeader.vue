<template>
    <div>
        <h1>Название сайта</h1>
        <a
        href="tel:+77777777777"
        @click="call"
        >+7 (777) 777 77 77</a>
    </div>
</template>

<script>
export default {
    methods: {
        call(event) {
            event.preventDefault();
            alert('Вы позвонили!');
        }
    }
}
</script>

<style scoped>
    div {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: rgb(233, 233, 233);
    }

    h1 {
        color: red;
    }
</style>