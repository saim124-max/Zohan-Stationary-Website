# Zohan-Station<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zohan Stationary - Your One-Stop Stationery Shop</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #271a1a;
            background-color: navy;
        }
        header {
            background-color: black;
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }
        .nav-links {
            list-style: none;
            display: flex;
        }
        .nav-links li {
            margin-left: 20px;
        }
        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: #ddd;
        }
        .menu-toggle {
            display: none;
            flex-direction: column;
            cursor: pointer;
        }
        .menu-toggle span {
            width: 25px;
            height: 3px;
            background-color: white;
            margin: 3px 0;
            transition: 0.3s;
        }
        main {
            margin-top: 80px;
        }
        section {
            padding: 60px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .hero {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://via.placeholder.com/1200x600?text=Stationery+Supplies') center/cover;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }
        .btn {
            display: inline-block;
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .btn:hover {
            background-color: #45a049;
        }
        .about, .products, .contact {
            background-color: white;
            margin: 20px 0;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .about h2, .products h2, .contact h2 {
            text-align: center;
            margin-bottom: 20px;
            color: #4CAF50;
        }
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .product {
            text-align: center;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 8px;
        }
        .product img {
            max-width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 8px;
        }
        .contact form {
            max-width: 500px;
            margin: 0 auto;
        }
        .contact input, .contact textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
        }
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                flex-direction: column;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: #4CAF50;
                padding: 20px 0;
            }
            .nav-links.active {
                display: flex;
            }
            .nav-links li {
                margin: 10px 0;
            }
            .menu-toggle {
                display: flex;
            }
            .hero h1 {
                font-size: 2rem;
            }
            .hero p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">Zohan Stationary</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="menu-toggle" onclick="toggleMenu()">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </nav>
    </header>

    <main>
        <section id="home" class="hero">
            <h1>Welcome to Zohan Stationary</h1>
            <p>Your one-stop shop for all stationery needs. Quality products at affordable prices.</p>
            <a href="#products" class="btn">Shop Now</a>
        </section>

        <section id="about" class="about">
            <h2>About Us</h2>
            <p>Zohan Stationary has been serving customers with high-quality stationery products for over 10 years. We offer a wide range of items including notebooks, pens, pencils, art supplies, and office essentials. Our commitment to quality and customer satisfaction sets us apart.</p>
        </section>

        <section id="products" class="products">
            <h2>Our Products</h2>
            <div class="products-grid">
                <div class="product">
                    <img src="https://via.placeholder.com/250x150?text=Notebooks" alt="Notebooks">
                    <h3>Notebooks</h3>
                    <p>High-quality notebooks for all your writing needs.</p>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/250x150?text=Pens+%26+Pencils" alt="Pens & Pencils">
                    <h3>Pens & Pencils</h3>
                    <p>Smooth writing pens and durable pencils.</p>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/250x150?text=Art+Supplies" alt="Art Supplies">
                    <h3>Art Supplies</h3>
                    <p>Everything you need for your creative projects.</p>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/250x150?text=Office+Essentials" alt="Office Essentials">
                    <h3>Office Essentials</h3>
                    <p>Staplers, paper clips, and more office supplies.</p>
                </div>
            </div>
        </section>

        <section id="contact" class="contact">
            <h2>Contact Us</h2>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" rows="5" required></textarea>
                <button type="submit" class="btn">Send Message</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Zohan Stationary. All rights reserved.</p>
    </footer>

    <script>
        function toggleMenu() {
            const navLinks = document.querySelector('.nav-links');
            navLinks.classList.toggle('active');
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>ary-Website
