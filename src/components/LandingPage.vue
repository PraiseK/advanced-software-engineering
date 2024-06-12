<template>
    <div>
        <header>
            <div class="container header-container">
                <div class="logo-container">
                    <img src="@/assets/logo.png" alt="Logo" class="logo">
                    <h1>Sikuta Australia</h1>
                </div>
                <nav>
                    <ul>
                        <li><router-link to="/signup" class="button">Sign Up</router-link></li>
                        <li><router-link to="/login" class="button">Login</router-link></li>
                    </ul>
                </nav>
            </div>
        </header>

        <section class="hero">
            <div class="container">
                <img src="@/assets/hero-vans.png" alt="Rental Vans">
                <form class="search-form">
                    <input type="text" placeholder="Pick Your Location">
                    <input type="date">
                    <input type="date">
                    <button type="submit">Search</button>
                </form>
            </div>
        </section>

        <section class="about">
            <div class="container">
                <h2>Who We Are</h2>
                <img src="@/assets/van.png" alt="Car">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vitae sapien eget nisl eleifend posuere.</p>
                <button>About Us</button>
            </div>
        </section>

        <section class="locations">
            <div class="container">
                <h2>Our Locations</h2>
                <div class="location">
                    <img src="@/assets/brisbane.jpg" alt="Brisbane">
                    <h3>Brisbane</h3>
                    <p>Get to explore Brisbane with our luxury cars. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                </div>
                <div class="location">
                    <img src="@/assets/townsville.jpg" alt="Townsville">
                    <h3>Townsville</h3>
                    <p>Get to explore Townsville with our luxury cars. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                </div>
            </div>
        </section>

        <footer>
            <div class="container">
                <p>&copy; 2024 Sikuta Car Rental. All rights reserved.</p>
                <nav>
                    <ul>
                        <li><router-link to="/about">About Us</router-link></li>
                        <li><router-link to="/payment">Payment Method</router-link></li>
                        <li><router-link to="/help">Help</router-link></li>
                        <li><router-link to="/order-status">Order Status</router-link></li>
                        <li><router-link to="/account">My Account</router-link></li>
                        <li><router-link to="/customer-service">Customer Service</router-link></li>
                    </ul>
                </nav>
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'LandingPage'
}
</script>

<style scoped>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

.container {
    width: 80%;
    margin: 0 auto;
    padding: 20px;
}

.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo-container {
    display: flex;
    align-items: center;
}

.logo {
    width: 50px;
    height: auto;
    margin-right: 10px;
}

header {
    background-color: #333;
    color: #fff;
    padding: 20px 0;
}

header h1 {
    margin: 0;
}

header nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    gap: 10px;
}

header nav ul li {
    margin-left: 20px;
}

header nav ul li .button {
    color: #fff;
    text-decoration: none;
    padding: 10px 20px;
    border-radius: 5px;
    background-color: #d9534f;
    transition: background-color 0.3s ease;
}

header nav ul li .button:hover {
    background-color: #c9302c;
}

.hero {
    background-color: #d9534f;
    text-align: center;
    padding: 40px 0;
}

.hero img {
    width: 100%;
    max-width: 600px;
    margin-bottom: 20px;
}

.search-form {
    display: flex;
    justify-content: center;
    gap: 10px;
}

.search-form input, .search-form button {
    padding: 10px;
    border: none;
    border-radius: 5px;
}

.search-form input {
    width: 150px;
}

.search-form button {
    background-color: #333;
    color: #fff;
}

.about {
    background-color: #fff;
    padding: 40px 0;
    text-align: center;
}

.about h2 {
    margin-bottom: 20px;
}

.about img {
    max-width: 100%;
    height: auto;
    margin-bottom: 20px;
}

.about p {
    max-width: 600px;
    margin: 0 auto 20px;
}

.about button {
    background-color: #d9534f;
    color: #fff;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
}

.locations {
    background-color: #fff;
    padding: 40px 0;
    text-align: center;
}

.locations h2 {
    margin-bottom: 40px;
}

.locations .location {
    display: inline-block;
    width: 45%;
    margin: 0 2.5%;
    text-align: left;
}

.locations .location img {
    width: 100%;
    height: auto;
    margin-bottom: 10px;
}

.locations .location h3 {
    margin-bottom: 10px;
}

.locations .location p {
    margin-bottom: 20px;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px 0;
}

footer nav ul {
    list-style: none;
    padding: 0;
    margin: 20px 0 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

footer nav ul li {
    margin: 5px 10px;
}

footer nav ul li a {
    color: #fff;
    text-decoration: none;
}
</style>
