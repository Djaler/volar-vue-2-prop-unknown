<template>
    <Child :value="innerValue"/>
</template>

<script lang="ts">
    import { defineComponent, ref } from '@vue/composition-api';
    import Child from '@/Child.vue';

    export default defineComponent({
        name: 'App',
        components: { Child },
        setup() {
            const innerValue = ref<unknown>(null);

            return {
                innerValue,
            };
        },
    });
</script>
