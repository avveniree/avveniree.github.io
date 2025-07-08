
<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8">
  <title>RELΛB‑style Shop</title>
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <div class="logo">RELΛB</div>
  <nav>
    <ul>
      <li><a href="#">CLOTHING</a>
        <div class="submenu">
          <a href="#">Hoodies</a>
          <a href="#">T‑shirts</a>
          <a href="#">Pants</a>
        </div>
      </li>
      <li><a href="#">ACCESSORIES</a>
        <div class="submenu">
          <a href="#">Bags</a>
          <a href="#">Hats</a>
          <a href="#">Sunglasses</a>
        </div>
      </li>
      <li><a href="#">COLLECTION</a>
        <div class="submenu">
          <a href="#">New Arrivals</a>
          <a href="#">Relab Classic</a>
          <a href="#">Summer</a>
        </div>
      </li>
    </ul>
  </nav>
  <div class="cart-search">
    <img src="https://cdn-icons-png.flaticon.com/512/622/622669.png" alt="Search">
    <img src="https://cdn-icons-png.flaticon.com/512/1170/1170678.png" alt="Cart">
  </div>
</header>

<section class="hero">
  <img src="https://via.placeholder.com/1200x400?text=Promocja+Nowych+Produkt%C3%B3w" alt="Baner" style="width:100%;">
</section>

<section class="products">
  <div class="product">
    <img src="https://via.placeholder.com/300x300?text=T-Shirt+RELΛB" alt="Produkt">
    <h3>"R" T‑Shirt</h3>
    <p>169,00 zł</p>
  </div>
  <div class="product">
    <img src="https://via.placeholder.com/300x300?text=Bluza+RELΛB" alt="Produkt">
    <h3>Faded Blue Hoodie</h3>
    <p>399,00 zł</p>
  </div>
</section>

<section class="newsletter">
  <div style="text-align:center; padding:20px;">
    <h2>DOŁĄCZ DO KLUBU RELAB</h2>
    <p>Zapisz się i zyskaj 10% rabatu</p>
    <input type="email" placeholder="Twój e‑mail">
    <button>Zapisz się</button>
  </div>
</section>

<footer>
  <p><a href="#">Regulamin</a> • <a href="#">Polityka prywatności</a> • <a href="#">Kontakt</a></p>
  <p>© 2025 All Rights Reserved RELAB®.</p>
</footer>

</body>
</html>
body {
  margin:0;
  font-family: sans-serif;
  background:#f9f9f9;
  color:#222;
}

header {
  display:flex;
  justify-content: space-between;
  align-items:center;
  padding:10px 20px;
  background:#fff;
  box-shadow:0 2px 5px rgba(0,0,0,0.1);
  position:sticky;
  top:0;
  z-index:100;
}

.logo {
  font-weight:bold;
  font-size:1.2rem;
}

nav ul {
  list-style:none;
  margin:0;
  padding:0;
  display:flex;
  gap:15px;
}

nav li {
  position:relative;
}

nav a {
  text-decoration:none;
  color:#222;
  padding:8px;
  display:block;
}

nav li:hover > .submenu {
  display:block;
}

.submenu {
  display:none;
  position:absolute;
  top:100%;
  left:0;
  background:#fff;
  box-shadow:0 2px 8px rgba(0,0,0,0.1);
  min-width:150px;
}

.submenu a {
  padding:10px;
}

.cart-search {
  display:flex;
  gap:15px;
  align-items:center;
}

.cart-search img {
  width:24px;
  height:24px;
  cursor:pointer;
}

.products {
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(200px,1fr));
  gap:20px;
  padding:20px;
  max-width:1200px;
  margin:auto;
}

.product {
  background:#fff;
  padding:10px;
  text-align:center;
  box-shadow:0 1px 4px rgba(0,0,0,0.1);
}

.product img {
  max-width:100%;
  height:auto;
}

footer {
  background:#fff;
  padding:20px;
  text-align:center;
  color:#777;
  box-shadow:0 -2px 5px rgba(0,0,0,0.05);
  margin-top:40px;
}

.newsletter input[type="email"] {
  padding:10px;
  width:200px;
  margin-right:10px;
  border:1px solid #ccc;
}

.newsletter button {
  padding:10px 16px;
  border:none;
  background:#222;
  color:#fff;
  cursor:pointer;
}
