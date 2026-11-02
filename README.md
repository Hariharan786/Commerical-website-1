
# Ex02 Commercial Website

## Date:2/11/26

## AIM

To create a commercial website using CSS Flexbox.

## ALGORITHM

### STEP 1

Create an HTML file (`index.html`).

### STEP 2

Create a CSS file (`style.css`).

### STEP 3

Include a navigation bar with links to different sections.

### STEP 4

Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5

Include social media links at the footer with copyright information.

### STEP 6

Define global styles for fonts, colors, and layout.

### STEP 7

Style the header, navigation bar, and sections.

### STEP 8

Use Flexbox for layout design.

### STEP 9

Add hover effects and transitions for interactivity.

### STEP 10

Add Images and Media.

### STEP 11

Use optimized images for a professional look.

### STEP 12

Open the HTML file in a browser to check layout and functionality.

### STEP 13

Fix styling issues and refine content placement.

### STEP 14

Deploy the website.

### STEP 15

Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav class="navbar">
            <div class="logo">TechStore</div>
            <ul class="nav-links">
                <li><a href="#">Home</a></li>
                <li><a href="#">Shop</a></li>
                <li><a href="#">Categories</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1>Welcome to TechStore</h1>
                <p>Upgrade your setup with premium gear at unbeatable prices.</p>
                <button class="cta-button">Shop Now</button>
            </div>
        </section>

        <section class="features">
            <div class="feature-box">
                <h3>Free Shipping</h3>
                <p>On all orders over ₹999</p>
            </div>
            <div class="feature-box">
                <h3>24/7 Support</h3>
                <p>We are here to help you</p>
            </div>
            <div class="feature-box">
                <h3>Easy Returns</h3>
                <p>30-day money-back guarantee</p>
            </div>
        </section>

        <h2 class="section-title">Featured Products</h2>
        <section class="products-container">
            <div class="product-card">
                <div class="product-image"></div>
                <h3>Wireless Headphones</h3>
                <p class="price">₹1,499</p>
                <button class="cart-btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <div class="product-image"></div>
                <h3>Mechanical Keyboard</h3>
                <p class="price">₹2,999</p>
                <button class="cart-btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <div class="product-image"></div>
                <h3>Gaming Mouse</h3>
                <p class="price">₹999</p>
                <button class="cart-btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <div class="product-image"></div>
                <h3>HD Monitor</h3>
                <p class="price">₹8,999</p>
                <button class="cart-btn">Add to Cart</button>
            </div>
        </section>
    </main>

    <footer>
        <div class="footer-content">
            <p>Hariharan Ganesh | Register Number: 212225040111</p>
            <div class="social-links">
                <a href="#">Facebook</a>
                <a href="#">Twitter</a>
                <a href="#">Instagram</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    background-color: #f4f7f6;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #1a252f;
    color: white;
    padding: 20px 5%;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
    letter-spacing: 1px;
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 25px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: #3498db;
}

main {
    flex-grow: 1;
}

.hero {
    background-color: #2c3e50;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 80px 20px;
}

.hero h1 {
    font-size: 2.5rem;
    margin-bottom: 15px;
}

.hero p {
    font-size: 1.1rem;
    margin-bottom: 25px;
}

.cta-button {
    padding: 12px 30px;
    font-size: 1rem;
    background-color: #e74c3c;
    color: white;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.cta-button:hover {
    background-color: #c0392b;
}

.features {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    padding: 40px 5%;
    background-color: white;
}

.feature-box {
    flex: 1;
    min-width: 250px;
    text-align: center;
    padding: 20px;
    background-color: #ecf0f1;
    border-radius: 8px;
}

.feature-box h3 {
    color: #2c3e50;
    margin-bottom: 10px;
}

.section-title {
    text-align: center;
    margin: 40px 0 20px;
    color: #2c3e50;
}

.products-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    padding: 0 5% 60px;
}

.product-card {
    background: white;
    padding: 20px;
    border-radius: 10px;
    width: 280px;
    text-align: center;
    display: flex;
    flex-direction: column;
    gap: 15px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: transform 0.3s;
}

.product-card:hover {
    transform: translateY(-5px);
}

.product-image {
    width: 100%;
    height: 180px;
    background-color: #bdc3c7;
    border-radius: 6px;
}

.price {
    font-weight: bold;
    font-size: 1.2rem;
    color: #e74c3c;
}

.cart-btn {
    padding: 10px;
    background-color: #3498db;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.cart-btn:hover {
    background-color: #2980b9;
}

footer {
    background-color: #1a252f;
    color: white;
    padding: 30px 5%;
    margin-top: auto;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
}

.social-links {
    display: flex;
    gap: 15px;
}

.social-links a {
    color: #bdc3c7;
    text-decoration: none;
}

.social-links a:hover {
    color: white;
}

@media (max-width: 768px) {
    .navbar, .footer-content {
        flex-direction: column;
        text-align: center;
    }
    
    .nav-links {
        margin-top: 15px;
        flex-wrap: wrap;
        justify-content: center;
    }
}
```
## OUTPUT

## OUTPUT



![Output Screenshot 1](ss1.png)


![Output Screenshot 2](ss2png)

## RESULT

The program for creating commercial website using CSS Flexbox is executed successfully.
