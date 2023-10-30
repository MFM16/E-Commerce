<template>
    <footer :class="[absolutePosition ? 'absolute bottom-0' : '']" class="w-full py-6 mt-6 text-center text-xs lg:text-sm text-slate-400 border-t-2 border-slate-300">
        2019 Copyright Store. All Rights Reserved.
    </footer>
</template>

<script>
    export default {
        name: 'FooterComponent',
        props: {
            absolutePosition:{
                type: Boolean,
                default: false
            }
        }
    }
</script>

<style scoped>

</style>