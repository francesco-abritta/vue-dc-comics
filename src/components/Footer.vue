<template>
    <div>
        <footer class="contenitore">
            <Merchandise />
            <Merchandise />
            <Merchandise />
            <Merchandise />
            <Merchandise />
        </footer>
    </div>
</template>

<script>
import Merchandise from './internFooter/Footer1/merchandise.vue'

export default {
    name: 'Footer',
    components: {
        Merchandise
    }
}
</script>

<style>
    footer{
        background-color: #117CEC;
        display: flex;
        justify-content: space-between;
    }
</style>