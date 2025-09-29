<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ShopEase - E-commerce Store</title>
  <style>
    /* Global Styles */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      background-color: #f5f5f5;
      color: #333;
    }

    /* Header */
    header {
      background-color: #2c3e50;
      color: white;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }
    header h1 {
      font-size: 28px;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: bold;
      transition: 0.3s;
    }
    nav a:hover {
      color: #e67e22;
    }
    .search-bar input {
      padding: 7px 10px;
      border-radius: 5px;
      border: none;
      width: 200px;
    }

    /* Categories */
    .categories {
      display: flex;
      justify-content: center;
      margin: 20px 0;
      gap: 15px;
      flex-wrap: wrap;
    }
    .categories button {
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      background-color: #3498db;
      color: white;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
    }
    .categories button:hover {
      background-color: #2980b9;
    }

    /* Product Grid */
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px 30px;
    }
    .product-card {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 15px;
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .product-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 16px rgba(0,0,0,0.2);
    }
    .product-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 10px;
    }
    .product-card h3 {
      margin: 10px 0;
      font-size: 18px;
    }
    .product-card p {
      color: #e74c3c;
      font-weight: bold;
      margin-bottom: 10px;
      font-size: 16px;
    }
    .product-card button {
      padding: 10px 15px;
      border: none;
      border-radius: 5px;
      background-color: #e74c3c;
      color: white;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
    }
    .product-card button:hover {
      background-color: #c0392b;
    }

    /* Footer */
    footer {
      background-color: #2c3e50;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }

    /* Responsive */
    @media(max-width: 600px) {
      .search-bar input {
        width: 100%;
        margin-top: 10px;
      }
      header {
        flex-direction: column;
        align-items: flex-start;
      }
      nav {
        margin-top: 10px;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>ShopEase</h1>
    <div class="search-bar">
      <input type="text" placeholder="Search products...">
    </div>
    <nav>
      <a href="#">Home</a>
      <a href="#">Categories</a>
      <a href="#">Cart</a>
      <a href="#">Profile</a>
    </nav>
  </header>

  <!-- Categories -->
  <div class="categories">
    <button>Electronics</button>
    <button>Clothing</button>
    <button>Books</button>
    <button>Home & Kitchen</button>
    <button>Sports</button>
  </div>

  <!-- Products -->
  <div class="products">
    <div class="product-card">
      <img src="https://via.placeholder.com/250x200" alt="Wireless Headphones">
      <h3>Wireless Headphones</h3>
      <p>$59.99</p>
      <button>Add to Cart</button>
    </div>
    <div class="product-card">
      <img src="https://via.placeholder.com/250x200" alt="Men's T-Shirt">
      <h3>Men's T-Shirt</h3>
      <p>$19.99</p>
      <button>Add to Cart</button>
    </div>
    <div class="product-card">
      <img src="https://via.placeholder.com/250x200" alt="Cookbook">
      <h3>Cookbook</h3>
      <p>$24.99</p>
      <button>Add to Cart</button>
    </div>
    <div class="product-card">
      <img src="https://via.placeholder.com/250x200" alt="Coffee Maker">
      <h3>Coffee Maker</h3>
      <p>$89.99</p>
      <button>Add to Cart</button>
    </div>
    <div class="product-card">
      <img src="https://via.placeholder.com/250x200" alt="Yoga Mat">
      <h3>Yoga Mat</h3>
      <p>$29.99</p>
      <button>Add to Cart</button>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    &copy; 2025 ShopEase. All Rights Reserved.
  </footer>

</body>
</html>
