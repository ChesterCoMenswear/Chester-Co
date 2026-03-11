<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chester & Co | Modern Menswear</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Lato:wght@300;400;500&display=swap" rel="stylesheet">

<style>

/* ------------------ GLOBAL ------------------ */

body {
  margin: 0;
  font-family: 'Lato', sans-serif;
  background-color: #F4EFE6;  /* Rich cream */
  color: #1A1A1A;
}

h1, h2, h3, h4 {
  font-family: 'Playfair Display', serif;
}

/* ------------------ HEADER & NAV ------------------ */

header {
  background-color: #0C1A30; /* Deep refined navy */
  padding: 22px 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
}

header h1 {
  margin: 0;
  font-size: 26px;
  letter-spacing: 1px;
}

nav {
  display: flex;
  gap: 40px;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  position: relative;
}

nav ul li {
  position: relative;
}

nav a {
  text-decoration: none;
  color: white;
  font-size: 15px;
  opacity: 0.9;
}

nav a:hover {
  opacity: 1;
}

.dropdown > a::after {
  content: " ▼";
  font-size: 11px;
  opacity: 0.6;
}

.dropdown-menu {
  display: none;
  position: absolute;
  background: white;
  color: black;
  border: 1px solid #ddd;
  padding: 10px 0;
  top: 28px;
  min-width: 160px;
}

.dropdown-menu a {
  display: block;
  padding: 10px 15px;
  color: #1A1A1A;
}

.dropdown-menu a:hover {
  background: #ECEBE6;
}

.dropdown:hover .dropdown-menu {
  display: block;
}

/* ------------------ HERO ------------------ */

.hero {
  height: 82vh;
  background: url('https://images.unsplash.com/photo-1490578474895-699cd4e2cf59?auto=format&fit=crop&w=1600&q=90')
              center/cover no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  text-align: center;
}

.hero h2 {
  font-size: 3rem;
  margin-bottom: 20px;
}

.hero button {
  padding: 13px 30px;
  background: #0C1A30;
  color: white;
  border: none;
  cursor: pointer;
  letter-spacing: 1px;
}

/* ------------------ COLLECTION GRID ------------------ */

section {
  padding: 80px 60px;
  max-width: 1200px;
  margin: auto;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 40px;
}

.item {
  background: white;
  border: 1px solid #D8D6D0;
  padding: 20px;
}

.item img {
  width: 100%;
  height: 330px;
  object-fit: cover;
}

.item h4 {
  margin-top: 12px;
  font-size: 1.2rem;
}

/* ------------------ FOOTER ------------------ */

.footer {
  background: #0C1A30;
  color: #D9D9D9;
  padding: 45px 30px;
  text-align: center;
  margin-top: 80px;
  font-size: 14px;
}

</style>
</head>


<body>

<!-- ====================== HEADER ====================== -->

<header>
  <h1>Chester & Co</h1>

  <nav>

    <!-- Clothing dropdown -->
    <ul class="dropdown">
      <li>
        <a href="#">Clothing</a>
        <ul class="dropdown-menu">
          <li><a href="#">Suits</a></li>
          <li><a href="#">Shirts</a></li>
          <li><a href="#">Trousers</a></li>
          <li><a href="#">Outerwear</a></li>
          <li><a href="#">Knitwear</a></li>
        </ul>
      </li>
    </ul>

    <!-- Accessories dropdown -->
    <ul class="dropdown">
      <li>
        <a href="#">Accessories</a>
        <ul class="dropdown-menu">
          <li><a href="#">Ties</a></li>
          <li><a href="#">Belts</a></li>
          <li><a href="#">Footwear</a></li>
          <li><a href="#">Bags</a></li>
        </ul>
      </li>
    </ul>

    <!-- About dropdown -->
    <ul class="dropdown">
      <li>
        <a href="#">About</a>
        <ul class="dropdown-menu">
          <li><a href="#">Our Story</a></li>
          <li><a href="#">Craftsmanship</a></li>
          <li><a href="#">Values</a></li>
        </ul>
      </li>
    </ul>

  </nav>
</header>

<!-- ====================== HERO ====================== -->

<div class="hero">
  <div>
    <h2>Modern Menswear, Redefined</h2>
    <button>Shop The Collection</button>
  </div>
</div>

<!-- ====================== COLLECTION GRID ====================== -->

<section>
  <div class="grid">

    <div class="item">
      <img src="https://images.unsplash.com/photo-1520975918318-3e7c7736e46e?auto=format&fit=crop&w=700&q=90">
      <h4>Suits</h4>
      <p>Sharp tailoring for a modern silhouette.</p>
    </div>

    <div class="item">
      <img src="https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?auto=format&fit=crop&w=700&q=90">
      <h4>Shirts</h4>
      <p>Premium cotton, refined details, everyday elegance.</p>
    </div>

    <div class="item">
      <img src="https://images.unsplash.com/photo-1600185365836-a568d43c036d?auto=format&fit=crop&w=700&q=90">
      <h4>Outerwear</h4>
      <p>Transitional layers designed with restraint and precision.</p>
    </div>

    <div class="item">
      <img src="https://images.unsplash.com/photo-1603349206295-a74f3e15f37a?auto=format&fit=crop&w=700&q=90">
      <h4>Accessories</h4>
      <p>Simple, refined essentials to elevate any fit.</p>
    </div>

  </div>
</section>

<!-- ====================== FOOTER ====================== -->

<div class="footer">
  © 2026 Chester & Co. All Rights Reserved.
</div>

</body>
</html>
