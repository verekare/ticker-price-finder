<template>
    <div class="ticker-list">
        <TickerItem
        v-for="t in tickers"
        :ticker="ticker"
        :key="t.id">
            {{ t.name }}
        </TickerItem>
    </div>
</template>

<script>
import TickerItem from './TickerItem.vue';

export default {
    components: {TickerItem},
    data() {
        return {
            tickers: {
                type: Array,
                required: true
            },
        }
    }
}
</script>

<style>
.ticker-list {
    margin: 60px;
    margin-top: 20px;
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}
</style>