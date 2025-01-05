<!DOCTYPE html>
<html>
<head>
    <title>Migt Shop Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            padding: 20px 10px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px 0;
        }
        nav a {
            margin: 0 15px;
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            color: #00bfff;
        }
        main {
            padding: 20px;
        }
        .category {
            margin: 20px 0;
        }
        .category h2 {
            cursor: pointer;
            color: #007BFF;
        }
        .category-details {
            display: none;
            padding: 10px;
            background-color: #e9e9e9;
            margin: 10px 0;
            border: 1px solid #ccc;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
    <script>
        function toggleDetails(id) {
            const element = document.getElementById(id);
            element.style.display = element.style.display === 'block' ? 'none' : 'block';
        }
    </script>
</head>
<body>
    <header>
        <h1>Migt Shop Website</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#product">Products</a>
        <a href="#contact">Contact</a>
    </nav>
    <main>
        <section id="home">
            <h2>Welcome to Our Website</h2>
            <p>Explore our amazing products and services.</p>
        </section>
        <section id="product">
            <h2>Our Products</h2>
            <div class="category">
                <h2 onclick="toggleDetails('category1')">Category 1</h2>
                <div id="category1" class="category-details">
                    <p>Details about Category 1 products.</p>
                </div>
            </div>
            <div class="category">
                <h2 onclick="toggleDetails('category2')">Category 2</h2>
                <div id="category2" class="category-details">
                    <p>Details about Category 2 products.</p>
                </div>
            </div>
            <div class="category">
                <h2 onclick="toggleDetails('category3')">Category 3</h2>
                <div id="category3" class="category-details">
                    <p>Details about Category 3 products.</p>
                </div>
            </div>
        </section>
        <section id="contact">
            <h2>Contact Us</h2>
            <p>For inquiries, visit our <a href="https://www.example.com" target="_blank">contact page</a>.</p>
        </section>
    </main>
    <footer>
        &copy; 2025 Migt Shop Website
    </footer>
</body>
</html>
