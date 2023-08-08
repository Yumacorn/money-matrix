<template>
    <div class="navigation">
        <span class="section">
            <a href="/"><button>Home</button></a>
        </span>
        <span class="section">
            <a href="/salary-calculator"><button>Salary Calculator (Disabled)</button></a>
        </span>
        <span class="section">
            <a href="/savings"><button>Savings</button></a>
            <button v-on:click="clickHandler">Click me</button>
        </span>
    </div>
</template>

<script>
    export default {
        name: 'NavBar',
        props: {
            experiment: String
        },
        methods: {
            clickHandler() {
                this.$emit('click');
            }
        }
    }
</script>

<style>
    .navigation {
        background-color: black;
        color: white;
        font-size: x-large;
        height: 40px;
    }

    .navigation .section {
        padding: 20px 20px;
    }
</style>