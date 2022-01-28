<template>
    <div>
        <div class="contenitore footer1">
            <Merchandise />
            <Merchandise />
            <Merchandise />
            <Merchandise />
            <Merchandise />
        </div>

        <div class="contenitore footer2">
            <Link />
        </div>

        <div class="contenitore footer3">
            <Social />
        </div>



    </div>
</template>

<script>
import Merchandise from './internFooter/Footer1/merchandise.vue'
import Link from './internFooter/Footer2/Link.vue'
import Social from './internFooter/Footer3/Social.vue'

export default {
    name: 'Footer',
    components: {
        Merchandise,
        Link,
        Social
    }
}
</script>

<style>
    .footer1{
        background-color: #117CEC;
        display: flex;
        justify-content: space-between;
    }

    .footer2{
        background-image: url('../assets/img/footer-bg.jpg');
    }

    .footer3{
        background-color: rgb(73, 73, 73);
    }


</style>