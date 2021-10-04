<template>
    {{value}}
</template>

<script lang="ts">
    import { defineComponent, PropType } from '@vue/composition-api';

    export default defineComponent({
        name: 'Child',
        props: {
            value: {
                type: Object as PropType<unknown>,
                default: null,
            },
        },
    });
</script>
