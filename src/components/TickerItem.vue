<template>
    <div class="item">
        <h3> {{ ticker }} - USD </h3>
        <p> {{  }} </p>
        <button>
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 25 25" fill="none">
            <g clip-path="url(#clip0_42_2)">
                <path d="M22.0659 0H2.9341C1.31594 0 0 1.31594 0 2.9341V22.0659C0 23.6841 1.31594 25 2.9341 25H22.0659C23.6841 25 25 23.6841 25 22.0659V2.9341C25 1.31594 23.6836 0 22.0659 0ZM24.022 22.0659C24.022 23.1447 23.1447 24.022 22.0659 24.022H2.9341C1.85533 24.022 0.978033 23.1447 0.978033 22.0659V2.9341C0.978033 1.85533 1.85533 0.978033 2.9341 0.978033H22.0659C23.1447 0.978033 24.022 1.85533 24.022 2.9341V22.0659ZM17.9914 7.70006L13.1917 12.4998L17.9914 17.2995C18.1826 17.4907 18.1826 17.7997 17.9914 17.9909C17.8961 18.0863 17.7709 18.1342 17.6457 18.1342C17.5205 18.1342 17.3953 18.0863 17.2999 17.9909L12.5002 13.1912L7.70055 17.9909C7.60519 18.0863 7.48 18.1342 7.35481 18.1342C7.22962 18.1342 7.10443 18.0863 7.00908 17.9909C6.81787 17.7997 6.81787 17.4907 7.00908 17.2995L11.8088 12.4998L7.00908 7.70006C6.81787 7.50885 6.81787 7.19979 7.00908 7.00859C7.20028 6.81738 7.50934 6.81738 7.70055 7.00859L12.5002 11.8083L17.2999 7.00859C17.4911 6.81738 17.8002 6.81738 17.9914 7.00859C18.1826 7.19979 18.1821 7.50885 17.9914 7.70006Z" fill="#454595"/>
            </g>
            <defs>
                <clipPath id="clip0_42_2">
                <rect width="25" height="25" fill="white"/>
                </clipPath>
            </defs>
            </svg>
            Удалить
        </button>
    </div>
</template>

<script>
export default {
    props: {
        ticker: {
            type: Object,
            name: 'DEMO',
            price: Number,
            required: true
        }
    },
}
</script>

<style scoped>
h3 {
    font-size: 1em;
}
p {
    font-size: 1.5em;
}
.item {
    max-width: 180px;
    min-width: 150px;
    border: 1px solid #454595;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
}
button {
    border-radius: 50px;
    border: 1px solid #454595;
    background: none;
    color: #454595;
    padding: 10px 15px;
    margin: 10px;
    margin-top: 40px;
}
</style>