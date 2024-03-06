<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="path/to/font-awesome/css/font-awesome.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        /* First Navigation Bar */
        .first-nav {
            display: flex;
            justify-content: space-between;
            background-color: #333;
            color: #fff;
            padding: 10px;
        }

        .nav-link {
            color: #fff;
            text-decoration: none;
            margin-right: 20px;
        }

        /* Second Navigation Bar */
        .second-nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #444;
            color: #fff;
            padding: 10px;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo img {
            max-height: 40px;
            margin-right: 10px;
        }

        .categories select {
            padding: 5px;
        }

        .search {
            display: flex;
        }

        .search input {
            padding: 5px;
            margin-right: 10px;
        }

        /* Third Navigation Bar */
        .third-nav {
            display: flex;
            justify-content: space-around;
            background-color: #555;
            color: #fff;
            padding: 10px;
        }

        /* Fourth Navigation Bar */
        .fourth-nav {
            display: flex;
            justify-content: space-around;
            background-color: #666;
            color: #fff;
            padding: 10px;
        }

        /* Slider Section */
        .slider {
            position: relative;
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            overflow: hidden;
        }

        .slider img {
            width: 100%;
            height: auto;
            display: none;
        }
/* Brand Section */
        .brand-section {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            overflow: hidden;
        }

        .brand-slider {
            display: flex;
            overflow-x: hidden;
            transition: transform 0.5s ease-in-out;
        }

        .brand-item {
            width: 100px; /* Adjust the width of each brand item as needed */
            margin-right: 20px;
        }

        .brand-item img {
            width: 100%;
            height: auto;
        }

        .slider-controls {
            display: flex;
            justify-content: space-between;
            margin-top: 10px;
        }

        .slider-controls button {
            background: #333;
            color: #fff;
            border: none;
            padding: 5px 10px;
            cursor: pointer;
        }

/* Hot Deal Section */
        .hot-deal-section {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            overflow: hidden;
        }

        .hot-deal-slider {
            display: flex;
            overflow-x: hidden;
            transition: transform 0.5s ease-in-out;
        }

        .product-item {
            width: 200px; /* Adjust the width of each product item as needed */
            margin-right: 20px;
            cursor: pointer;
        }

        .product-item img {
            width: 100%;
            height: auto;
        }

        .product-info {
            text-align: center;
            margin-top: 10px;
        }

/* Section Hover Effect */
        .section-container {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }

        .section-item {
            position: relative;
            width: 200px;
            overflow: hidden;
        }

        .section-item img {
            width: 100%;
            height: auto;
        }

        .section-name {
            position: absolute;
            bottom: 0;
            background-color: rgba(0, 0, 0, 0.7);
            color: #fff;
            width: 100%;
            text-align: center;
            padding: 10px;
            opacity: 0;
            transition: opacity 0.3s ease-in-out;
        }

        .section-item:hover .section-name {
            opacity: 1;
        }

/* Phone Section */
        .phone-section {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #eee;
            padding: 20px;
        }

        .phone-image {
            width: 40%;
            max-width: 400px;
        }

        .phone-info {
            width: 50%;
            max-width: 500px;
        }

        .phone-info h2 {
            font-size: 24px;
            margin-bottom: 10px;
        }

        .phone-info p {
            font-size: 16px;
            margin-bottom: 20px;
        }

        .phone-number {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .phone-number input {
            padding: 10px;
            width: 70%;
            margin-right: 10px;
        }

        .get-app-button {
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }

        .app-store-links {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }

        .app-store-links img {
            height: 40px;
        }

/* What Clients Say Section */
        .clients-say-section {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            display: flex;
            justify-content: space-between;
            background-color: #eee;
            padding: 20px;
        }

        .client-box {
            width: 30%;
            padding: 20px;
            border: 1px solid #ccc;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

        .quote {
            font-size: 18px;
            margin-bottom: 15px;
        }

        .client-name {
            font-weight: bold;
        }

/* New Sections */
        .new-sections {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            display: flex;
            justify-content: space-between;
            background-color: #eee;
            padding: 20px;
        }

        .section-box {
            width: 22%;
            padding: 20px;
            border: 1px solid #ccc;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

        .box-icon {
            font-size: 36px;
            margin-bottom: 15px;
        }

        .box-title {
            font-size: 18px;
            margin-bottom: 15px;
            font-weight: bold;
        }

        .box-description {
            font-size: 14px;
        }
/* Boxes Layout */
        .boxes-layout {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            background-color: #eee;
            padding: 20px;
        }

        .box {
            width: 48%; /* Adjust the width as needed */
            margin-bottom: 20px;
            padding: 20px;
            border: 1px solid #ccc;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

/* Newsletter Section */
        .newsletter-section {
            width: 100%;
            max-width: 1200px;
            margin: 20px auto;
            text-align: center;
            background-color: #eee;
            padding: 20px;
        }

        .newsletter-title {
            font-size: 24px;
            font-weight: bold;
            color: #007BFF; /* Blue color */
            margin-bottom: 20px;
        }

        .newsletter-description {
            font-size: 16px;
            margin-bottom: 20px;
        }

        .email-input {
            padding: 10px;
            width: 60%;
            margin-right: 10px;
        }

        .subscribe-button {
            background-color: #007BFF; /* Blue color */
            color: #fff;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }

/* Footer Styles */
        footer {
            width: 100%;
            background-color: #333;
            color: #fff;
            padding: 20px;
        }

        .footer-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }

        .footer-section {
            width: 30%; /* Adjust the width as needed */
            margin-bottom: 20px;
        }

        .footer-section h3 {
            font-size: 18px;
            margin-bottom: 10px;
        }

        .footer-section ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        .footer-section ul li {
            margin-bottom: 10px;
        }

        .footer-social-icons {
            margin-top: 20px;
            display: flex;
            justify-content: space-between;
        }

        .footer-social-icons a {
            color: #fff;
            text-decoration: none;
            font-size: 24px;
            margin-right: 10px;
        }

        /* Add more custom styles as needed */

    </style>
    <title>Your Website</title>
</head>
<body>

<!-- First Navigation Bar -->
<nav class="first-nav">
    <div class="left-side">
        <a href="#" class="nav-link"><i class="fa fa-download"></i> Download App</a>
        <a href="#" class="nav-link"><i class="fa fa-phone"></i> Phone Number</a>
        <a href="#" class="nav-link"><i class="fa fa-whatsapp"></i> WhatsApp Number</a>
    </div>
    <div class="right-side">
        <a href="#" class="nav-link">Get a Free Quote</a>
        <a href="#" class="nav-link">Become a Seller</a>
        <a href="#" class="nav-link">Login</a>
        <a href="#" class="nav-link">Register</a>
    </div>
</nav>

<!-- Second Navigation Bar -->
<nav class="second-nav">
    <div class="logo">
        <a href="#"><img src="path/to/your-logo.png" alt="Logo"></a>
        <span>Company Name</span>
    </div>
    <div class="categories">
        <select>
            <option>Category 1</option>
            <option>Category 2</option>
        </select>
    </div>
    <div class="search">
        <input type="text" placeholder="Search">
        <button>Search</button>
    </div>
    <div class="actions">
        <a href="#" class="nav-link">Become a Seller</a>
        <a href="#" class="nav-link"><i class="fa fa-shopping-cart"></i> Cart</a>
    </div>
    <div class="create-website">
        <a href="#" class="nav-link">Create a Website</a>
    </div>
</nav>

<!-- Third Navigation Bar -->
<nav class="third-nav">
    <a href="#" class="nav-link">Cement</a>
    <a href="#" class="nav-link">Brands</a>
    <a href="#" class="nav-link">Buying Guide</a>
    <a href="#" class="nav-link">Best Selling</a>
    <a href="#" class="nav-link">Material Calculator</a>
</nav>

<!-- Fourth Navigation Bar -->
<nav class="fourth-nav">
    <a href="#" class="nav-link">Cement</a>
    <a href="#" class="nav-link">TMT Steels</a>
    <a href="#" class="nav-link">Paints</a>
    <a href="#" class="nav-link">Plumbing</a>
    <a href="#" class="nav-link">Tiles</a>
    <a href="#" class="nav-link">Lighting and Fixtures</a>
</nav>

<!-- Slider Section -->
<div class="slider">
    <!-- Placeholder content, replace with your actual slider content -->
    <img src="path/to/slider-image1.jpg" alt="Slider Image 1">
    <img src="path/to/slider-image2.jpg" alt="Slider Image 2">
    <img src="path/to/slider-image3.jpg" alt="Slider Image 3">
</div>

<!-- Add your additional HTML content here -->

<script>
    // JavaScript for automatic slider
    let currentIndex = 0;
    const slides = document.querySelectorAll('.slider img');
    const intervalTime = 1000; // 3 seconds

    function nextSlide() {
        slides[currentIndex].style.display = 'none';
        currentIndex = (currentIndex + 1) % slides.length;
        slides[currentIndex].style.display = 'block';
    }

    function startSlider() {
        setInterval(nextSlide, intervalTime);
    }

    // Initial call to start the slider
    startSlider();
</script>

<div class="brand-section">
    <div class="brand-slider">
        <!-- Placeholder content, replace with your actual brand images -->
        <div class="brand-item"><img src="path/to/brand1.jpg" alt="Brand 1"></div>
        <div class="brand-item"><img src="path/to/brand2.jpg" alt="Brand 2"></div>
        <div class="brand-item"><img src="path/to/brand3.jpg" alt="Brand 3"></div>
        <div class="brand-item"><img src="path/to/brand4.jpg" alt="Brand 4"></div>
        <div class="brand-item"><img src="path/to/brand5.jpg" alt="Brand 5"></div>
        <div class="brand-item"><img src="path/to/brand6.jpg" alt="Brand 6"></div>
        <div class="brand-item"><img src="path/to/brand7.jpg" alt="Brand 7"></div>
        <div class="brand-item"><img src="path/to/brand8.jpg" alt="Brand 8"></div>
    </div>
    <div class="slider-controls">
        <button onclick="prevBrand()">&#60;</button>
        <button onclick="nextBrand()">&#62;</button>
        <button onclick="viewAllBrands()">View All</button>
    </div>
</div>

<!-- Add your additional HTML content here -->

<script>
    // JavaScript for brand slider
    const brandSlider = document.querySelector('.brand-slider');
    let brandIndex = 0;
    const brandItems = document.querySelectorAll('.brand-item');
    const brandItemWidth = brandItems[0].offsetWidth;
    const totalBrands = brandItems.length;

    function nextBrand() {
        if (brandIndex < totalBrands - 1) {
            brandIndex++;
        } else {
            brandIndex = 0;
        }
        updateBrandSlider();
    }

    function prevBrand() {
        if (brandIndex > 0) {
            brandIndex--;
        } else {
            brandIndex = totalBrands - 1;
        }
        updateBrandSlider();
    }

    function updateBrandSlider() {
        brandSlider.style.transform = `translateX(${-brandIndex * brandItemWidth}px)`;
    }

    function viewAllBrands() {
        // Implement logic for the "View All" button
        // You can redirect to a separate page or display a modal, etc.
        console.log('View All Brands clicked!');
    }

    function autoSlideBrand() {
        setInterval(nextBrand, 3000); // Auto slide every 3 seconds
    }

    // Initial call to start the brand slider
    autoSlideBrand();
</script>

<!-- Hot Deal Section -->
<div class="hot-deal-section">
    <div class="hot-deal-slider">
        <!-- Placeholder content, replace with your actual product information -->
        <div class="product-item">
            <img src="path/to/product1.jpg" alt="Product 1">
            <div class="product-info">
                <p>Product Name 1</p>
                <p>Sale Price: Rs 38</p>
                <p>Upto 5% Off</p>
            </div>
        </div>
        <div class="product-item">
            <img src="path/to/product2.jpg" alt="Product 2">
            <div class="product-info">
                <p>Product Name 2</p>
                <p>Sale Price: Rs 38</p>
                <p>Upto 5% Off</p>
            </div>
        </div>
        <!-- Repeat the structure for other products -->
    </div>
    <div class="slider-controls">
        <button onclick="prevProduct()">&#60;</button>
        <button onclick="nextProduct()">&#62;</button>
    </div>
</div>

<!-- Add your additional HTML content here -->

<!-- Hot Deal Section -->
<div class="hot-deal-section">
    <div class="hot-deal-slider">
        <!-- Placeholder content, replace with your actual product information -->
        <!-- ... -->
    </div>
    <div class="slider-controls">
        <button onclick="prevProduct()">&#60;</button>
        <button onclick="nextProduct()">&#62;</button>
    </div>
</div>

<!-- Section Images with Hover Effect -->
<div class="section-container">
    <div class="section-item">
        <img src="path/to/bricks-image.jpg" alt="Bricks Image">
        <div class="section-name">Bricks</div>
    </div>
    <div class="section-item">
        <img src="path/to/steel-image.jpg" alt="Steel Image">
        <div class="section-name">Steel</div>
    </div>
    <div class="section-item">
        <img src="path/to/cement-image.jpg" alt="Cement Image">
        <div class="section-name">Cement</div>
    </div>
</div>

<script>
    // JavaScript for hot deal slider
    const productSlider = document.querySelector('.hot-deal-slider');
    let productIndex = 0;
    const productItems = document.querySelectorAll('.product-item');
    const productItemWidth = productItems[0].offsetWidth;
    const totalProducts = productItems.length;

    function nextProduct() {
        if (productIndex < totalProducts - 1) {
            productIndex++;
        } else {
            productIndex = 0;
        }
        updateProductSlider();
    }

    function prevProduct() {
        if (productIndex > 0) {
            productIndex--;
        } else {
            productIndex = totalProducts - 1;
        }
        updateProductSlider();
    }

    function updateProductSlider() {
        productSlider.style.transform = `translateX(${-productIndex * productItemWidth}px)`;
    }
</script>

<!-- Phone Section -->
<div class="phone-section">
    <div class="phone-image">
        <img src="path/to/phone-image.jpg" alt="Phone Image">
    </div>
    <div class="phone-info">
        <h2>Get Our App</h2>
        <p>Get deals and more! Search products and get verified seller info.</p>
        <div class="phone-number">
            <input type="tel" placeholder="Enter your phone number">
            <button class="get-app-button">Get App Now</button>
        </div>
        <div class="app-store-links">
            <a href="#" target="_blank"><img src="path/to/google-play-badge.png" alt="Get it on Google Play"></a>
            <a href="#" target="_blank"><img src="path/to/app-store-badge.png" alt="Available on the App Store"></a>
        </div>
    </div>
</div>

<!-- What Clients Say Section -->
<div class="clients-say-section">
    <div class="client-box">
        <div class="quote">"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio."</div>
        <div class="client-name">Client 1</div>
    </div>
    <div class="client-box">
        <div class="quote">"Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas."</div>
        <div class="client-name">Client 2</div>
    </div>
    <div class="client-box">
        <div class="quote">"Suspendisse potenti. Sed ac leo et justo tincidunt dapibus."</div>
        <div class="client-name">Client 3</div>
    </div>
</div>

<!-- New Sections -->
<div class="new-sections">
    <div class="section-box">
        <i class="fa fa-credit-card box-icon"></i>
        <div class="box-title">100% SECURE PAYMENTS</div>
        <div class="box-description">Moving your card details to a much more secured place</div>
    </div>
    <div class="section-box">
        <i class="fa fa-shield box-icon"></i>
        <div class="box-title">TRUST PAY</div>
        <div class="box-description">100% Payment Protection. Your money is safe with us.</div>
    </div>
    <div class="section-box">
        <i class="fa fa-truck box-icon"></i>
        <div class="box-title">SHIPPING</div>
        <div class="box-description">Free shipping on all orders (Subject to order value).</div>
    </div>
    <div class="section-box">
        <i class="fa fa-life-ring box-icon"></i>
        <div class="box-title">SUPPORT 24/7</div>
        <div class="box-description">We support online/offline 24/7. Reach out to us anytime.</div>
    </div>
</div>

<!-- Boxes Layout -->
<div class="boxes-layout">
    <!-- Horizontal Boxes -->
    <div class="box">
        <h2>Post Your Requirement</h2>
    </div>
    <div class="box">
        <h2>Become a Seller</h2>
    </div>
    <div class="box">
        <h2>Get a Free Quote</h2>
    </div>
    <div class="box">
        <h2>Contact Us</h2>
    </div>

    <!-- Vertical Boxes -->
    <div class="box" style="width: 100%;">
        <h2>Credit Request</h2>
    </div>
    <div class="box" style="width: 100%;">
        <h2>Builder Custom Home</h2>
    </div>
    <div class="box" style="width: 100%;">
        <h2>Advertise With Us</h2>
    </div>
    <div class="box" style="width: 100%;">
        <h2>Services</h2>
    </div>
</div>

<!-- Newsletter Section -->
<div class="newsletter-section">
    <div class="newsletter-title">Join Our Newsletter</div>
    <div class="newsletter-description">
        Register now to get the latest price updates on promotions and coupons.
    </div>
    <form action="#" method="post"> <!-- Add your form action -->
        <input type="email" class="email-input" placeholder="Please enter your email address" name="email" required>
        <button type="submit" class="subscribe-button">Subscribe</button>
    </form>
</div>

<!-- Footer Section -->
<footer>
    <div class="footer-container">

        <!-- First Footer -->
        <div class="footer-section">
            <h3>Testimonials</h3>
            <ul>
                <li>Services</li>
                <li>Sellers</li>
                <li>Interiors</li>
                <li>Build Your Home</li>
                <li>Post Your Requirement</li>
                <li>Contact Us</li>
            </ul>
        </div>

        <!-- Second Footer -->
        <div class="footer-section">
            <h3>Popular Searches</h3>
            <ul>
                <!-- Add your list items here -->
            </ul>
        </div>

        <!-- Third Footer -->
        <div class="footer-section">
            <h3>Contact Us</h3>
            <p>BuildersMart<br>#8-10, Fortune Chambers,<br>Image Gardens Lane, Hi-Tech City,<br>Madhapur, Hyderabad-500081.<br>Telangana.</p>
            <p>Phone: 9339330099</p>
            <p>WhatsApp: +91 9339330099</p>
            <p>Email: info@buildersmart.in</p>
        </div>

        <!-- Fourth Footer -->
        <div class="footer-section">
            <h3>Payment</h3>
            <!-- Add payment icons here -->
            <div class="footer-social-icons">
                <i class="fa fa-cc-visa"></i>
                <i class="fa fa-cc-mastercard"></i>
                <!-- Add more payment icons as needed -->
            </div>

            <h3>Follow Us</h3>
            <div class="footer-social-icons">
                <a href="#" target="_blank"><i class="fa fa-facebook"></i></a>
                <a href="#" target="_blank"><i class="fa fa-twitter"></i></a>
                <a href="#" target="_blank"><i class="fa fa-instagram"></i></a>
                <a href="#" target="_blank"><i class="fa fa-linkedin"></i></a>
            </div>
        </div>

        <!-- Fifth Footer -->
        <div class="footer-section" style="width: 100%;">
            <p>Copyright © 2020 BuildersMART. All Rights Reserved.</p>
        </div>

    </div>
</footer>




<script>
    // You can add JavaScript functionality here if needed
</script>

</body>
</html>
