<template>
    <div>
        <button
            @click="show = !show"
        >
            {{ buttonTitle }}
        </button>
        <template v-if="show">
            <p>{{ text }}</p>
            <input
                type="text"
                v-model="text"
            >
        </template>
    </div>
</template>

<script>
export default {
    data() {
        return {
            text: '',
            show: true
        }
    },
    computed: {
        buttonTitle() {
            if (this.show) {
                return 'Скрыть';
            } else {
                return 'Показать'
            }
        }
    }
}
</script>