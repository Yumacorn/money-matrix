<template>
    <div class="footer">
        <p>
            <span>&copy; 2023 Ryan Mui</span><a href="/contact"><button>Contact Us</button></a>
        </p>
    </div>
</template>

<script>
    export default {
        name: 'FooterBar',
    }
</script>

<style>
    .footer {
        background-color: teal;
        color: black;
        height: 30px;   
    }

    .footer span {
        padding: 0px 20px;
        vertical-align: auto;
    }
</style>