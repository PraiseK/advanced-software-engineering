<template>
    
    <div class="nav">
        <img src="../assets/logo.png">
        <a href="#">Login</a>
        <a href="#">Contact</a>
        <a href="#">About us</a>
        <a href="#">Home</a>
    </div>
</template>

<script>
    export default {
        name: 'HeaderBanner'
    }
</script>

<style>
    .nav {
        background-color: #333;
        overflow: hidden;

    }

    body {
        padding: 0;
        margin: 0;
        
    }

    .nav a {
        float: right;
        color: rgb(250, 68, 68);
        padding: 14px 16px;
        margin-top: 10px;
        font-size: 23px;
        text-decoration: none;
        margin-right: 5px;
        text-align: center;
    }

    .nav a:hover {
        background-color: #ddd;
        color: #333;
    }

    .nav img {
        padding: 0;
        margin-left: 25px;
        float: left;
        max-width: 5%;
    }
</style>