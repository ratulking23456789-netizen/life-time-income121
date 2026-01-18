<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>আমার শপ - অনলাইন শপিং</title>
    <style>
        /* CSS - সাইটের ডিজাইন */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 15px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }
        .container {
            width: 80%;
            margin: 20px auto;
        }
        h2 {
            text-align: center;
            color: #333;
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .product-card {
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }
        .product-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
        }
        .price {
            color: #e67e22;
            font-size: 18px;
            font-weight: bold;
            margin: 10px 0;
        }
        button {
            background-color: #27ae60;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #219150;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <header>
        <h1>আমার শপ (My Shop)</h1>
    </header>

    <nav>
        <a href="#">হোম</a>
        <a href="#">প্রোডাক্টস</a>
        <a href="#">কার্ট (<span id="cart-count">0</span>)</a>
        <a href="#">লগইন</a>
    </nav>

    <div class="container">
        <h2>জনপ্রিয় পণ্যসমূহ</h2>
        
        <div class="product-grid">
            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>স্মার্ট ওয়াচ</h3>
                <p>সেরা মানের ওয়াটারপ্রুফ স্মার্ট ওয়াচ।</p>
                <div class="price">৳ ১,৫০০</div>
                <button onclick="addToCart('স্মার্ট ওয়াচ', 1500)">কার্টে যোগ করুন</button>
            </div>

            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>হেডফোন</h3>
                <p>নয়েজ ক্যানসেলেশন সহ অরিজিনাল হেডফোন।</p>
                <div class="price">৳ ৮৫০</div>
                <button onclick="addToCart('হেডফোন', 850)">কার্টে যোগ করুন</button>
            </div>

            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>স্নিকার্স জুতা</h3>
                <p>স্টাইলিশ এবং আরামদায়ক রানিং সু।</p>
                <div class="price">৳ ২,২০০</div>
                <button onclick="addToCart('স্নিকার্স জুতা', 2200)">কার্টে যোগ করুন</button>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; ২০২৪ আমার শপ। সর্বস্বত্ব সংরক্ষিত।</p>
    </footer>

    <script>
        // JavaScript - কার্ট ফাংশনালিটি
        let cartCount = 0;

        function addToCart(productName, price) {
            cartCount++;
            document.getElementById('cart-count').innerText = cartCount;
            alert(productName + " সফলভাবে কার্টে যোগ করা হয়েছে! দাম: ৳" + price);
        }
    </script><!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>আমার শপ - অনলাইন শপিং</title>
    <style>
        /* CSS - সাইটের ডিজাইন */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 15px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }
        .container {
            width: 80%;
            margin: 20px auto;
        }
        h2 {
            text-align: center;
            color: #333;
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .product-card {
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }
        .product-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
        }
        .price {
            color: #e67e22;
            font-size: 18px;
            font-weight: bold;
            margin: 10px 0;
        }
        button {
            background-color: #27ae60;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #219150;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <header>
        <h1>আমার শপ (My Shop)</h1>
    </header>

    <nav>
        <a href="#">হোম</a>
        <a href="#">প্রোডাক্টস</a>
        <a href="#">কার্ট (<span id="cart-count">0</span>)</a>
        <a href="#">লগইন</a>
    </nav>

    <div class="container">
        <h2>জনপ্রিয় পণ্যসমূহ</h2>
        
        <div class="product-grid">
            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>স্মার্ট ওয়াচ</h3>
                <p>সেরা মানের ওয়াটারপ্রুফ স্মার্ট ওয়াচ।</p>
                <div class="price">৳ ১,৫০০</div>
                <button onclick="addToCart('স্মার্ট ওয়াচ', 1500)">কার্টে যোগ করুন</button>
            </div>

            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>হেডফোন</h3>
                <p>নয়েজ ক্যানসেলেশন সহ অরিজিনাল হেডফোন।</p>
                <div class="price">৳ ৮৫০</div>
                <button onclick="addToCart('হেডফোন', 850)">কার্টে যোগ করুন</button>
            </div>

            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>স্নিকার্স জুতা</h3>
                <p>স্টাইলিশ এবং আরামদায়ক রানিং সু।</p>
                <div class="price">৳ ২,২০০</div>
                <button onclick="addToCart('স্নিকার্স জুতা', 2200)">কার্টে যোগ করুন</button>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; ২০২৪ আমার শপ। সর্বস্বত্ব সংরক্ষিত।</p>
    </footer>

    <script>
        // JavaScript - কার্ট ফাংশনালিটি
        let cartCount = 0;

        function addToCart(productName, price) {
            cartCount++;
            document.getElementById('cart-count').innerText = cartCount;
            alert(productName + " সফলভাবে কার্টে যোগ করা হয়েছে! দাম: ৳" + price);
        }
    </script><!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>আমার শপ - অনলাইন শপিং</title>
    <style>
        /* CSS - সাইটের ডিজাইন */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 15px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }
        .container {
            width: 80%;
            margin: 20px auto;
        }
        h2 {
            text-align: center;
            color: #333;
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .product-card {
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }
        .product-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
        }
        .price {
            color: #e67e22;
            font-size: 18px;
            font-weight: bold;
            margin: 10px 0;
        }
        button {
            background-color: #27ae60;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #219150;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <header>
        <h1>আমার শপ (My Shop)</h1>
    </header>

    <nav>
        <a href="#">হোম</a>
        <a href="#">প্রোডাক্টস</a>
        <a href="#">কার্ট (<span id="cart-count">0</span>)</a>
        <a href="#">লগইন</a>
    </nav>

    <div class="container">
        <h2>জনপ্রিয় পণ্যসমূহ</h2>
        
        <div class="product-grid">
            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>স্মার্ট ওয়াচ</h3>
                <p>সেরা মানের ওয়াটারপ্রুফ স্মার্ট ওয়াচ।</p>
                <div class="price">৳ ১,৫০০</div>
                <button onclick="addToCart('স্মার্ট ওয়াচ', 1500)">কার্টে যোগ করুন</button>
            </div>

            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>হেডফোন</h3>
                <p>নয়েজ ক্যানসেলেশন সহ অরিজিনাল হেডফোন।</p>
                <div class="price">৳ ৮৫০</div>
                <button onclick="addToCart('হেডফোন', 850)">কার্টে যোগ করুন</button>
            </div>

            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Product Image">
                <h3>স্নিকার্স জুতা</h3>
                <p>স্টাইলিশ এবং আরামদায়ক রানিং সু।</p>
                <div class="price">৳ ২,২০০</div>
                <button onclick="addToCart('স্নিকার্স জুতা', 2200)">কার্টে যোগ করুন</button>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; ২০২৪ আমার শপ। সর্বস্বত্ব সংরক্ষিত।</p>
    </footer>

    <script>
        // JavaScript - কার্ট ফাংশনালিটি
        let cartCount = 0;

        function addToCart(productName, price) {
            cartCount++;
            document.getElementById('cart-count').innerText = cartCount;
            alert(productName + " সফলভাবে কার্টে যোগ করা হয়েছে! দাম: ৳" + price);
        }
    </script>
