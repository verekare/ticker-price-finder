<template>
<h3>Тикер</h3>
<div class="input-add">
    <input 
    v-model="ticker"
    v-on:keydown.enter="add"
    type="text" placeholder="Например, DOGE">
    <button @click="add">
        <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 25 25" fill="none">
        <circle cx="12.5" cy="12.5" r="12" stroke="#FFF"/>
        <line x1="12.5" y1="6" x2="12.5" y2="19" stroke="#FFF"/>
        <line x1="19" y1="12.5" x2="6" y2="12.5" stroke="#FFF"/>
        </svg>    
        Добавить
    </button>
</div>
</template>

<script>
export default {
    data() {
        return {
            ticker: 'default'
        }
    },
    methods: {
        add(event) {
            alert(this.ticker)
        }
    }
}
</script>

<style>
h3 {
    margin: 30px auto;
}
.input-add {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    display: flex;
    gap: 15px;
    justify-content: center;
}
input {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    padding: 10px 15px;
    border: none;
    border-bottom: 1px solid rgb(69, 69, 149);
}
button {
    padding: 10px 15px;
    border: none;
    color: whitesmoke;
    display: flex;
    align-items: center;
    gap: 8px;
    background-color: rgb(69, 69, 149);
    border-radius: 50px;
}
</style>