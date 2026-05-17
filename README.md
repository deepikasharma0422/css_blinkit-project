/* Created by Dipika Sharma */

<!DOCTYPE html>
<html>
<head>
<title>Blinkit Clone - Dipika Sharma</title>

<style>
body {
    margin: 0;
    font-family: Arial;
    background: #f5f5f5;
}

/* HEADER */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #0c8f3f;
    color: white;
    padding: 15px;
}

.logo {
    font-size: 22px;
    font-weight: bold;
}

header input {
    width: 40%;
    padding: 8px;
    border-radius: 5px;
    border: none;
}

/* BANNER */
.banner img {
    width: 100%;
    height: 250px;
    object-fit: cover;
}

/* CATEGORY SECTION */
.categories {
    display: flex;
    gap: 10px;
    padding: 15px;
    overflow-x: auto;
}

.cat {
    background: white;
    padding: 10px;
    border-radius: 10px;
    text-align: center;
    min-width: 100px;
    cursor: pointer;
}

.cat img {
    width: 60px;
    height: 60px;
}

/* PRODUCTS */
.section-title {
    padding: 10px 15px;
}

.container {
    display: grid;
    grid-template-columns: repeat(4,1fr);
    gap: 10px;
    padding: 10px;
}

.card {
    background: white;
    padding: 10px;
    border-radius: 10px;
    text-align: center;
}

.card img {
    width: 100%;
    height: 120px;
    object-fit: cover;
}

button {
    background: #0c8f3f;
    color: white;
    border: none;
    padding: 8px;
    margin-top: 5px;
    border-radius: 5px;
    cursor: pointer;
}

/* PORTFOLIO */
.portfolio {
    background: white;
    margin: 20px;
    padding: 20px;
    border-radius: 10px;
}

.profile {
    display: flex;
    gap: 20px;
    align-items: center;
}

.profile img {
    width: 120px;
    border-radius: 50%;
}

/* FOOTER */
footer {
    background: #222;
    color: white;
    text-align: center;
    padding: 10px;
}
</style>

</head>

<body>

<!-- HEADER -->
<header>
    <div class="logo">Blinkit</div>
    <input type="text" placeholder="Search 'milk'">
</header>

<!-- REALISTIC BANNER -->
<section class="banner">
    <img src="https://images.unsplash.com/photo-1607082348824-0a96f2a4b9da?q=80&w=1200" alt="">
</section>

<!-- CATEGORIES (LIKE BLINKIT) -->
<div class="categories">

    <div class="cat">
        <img src="https://cdn-icons-png.flaticon.com/512/135/135620.png">
        <p>Fruits</p>
    </div>

    <div class="cat">
        <img src="https://cdn-icons-png.flaticon.com/512/3075/3075977.png">
        <p>Vegetables</p>
    </div>

    <div class="cat">
        <img src="https://cdn-icons-png.flaticon.com/512/1046/1046784.png">
        <p>Dairy</p>
    </div>

    <div class="cat">
        <img src="https://cdn-icons-png.flaticon.com/512/3081/3081559.png">
        <p>Snacks</p>
    </div>

    <div class="cat">
        <img src="https://cdn-icons-png.flaticon.com/512/2935/2935307.png">
        <p>Beverages</p>
    </div>

</div>

<!-- GROCERIES -->
<h2 class="section-title">Popular Groceries</h2>

<div class="container">

    <div class="card">
        <img src="https://images.unsplash.com/photo-1567306226416-28f0efdc88ce">
        <h3>Banana</h3>
        <p>₹40/dozen</p>
        <button onclick="addToCart('Banana')">Add</button>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b">
        <h3>Milk</h3>
        <p>₹50</p>
        <button onclick="addToCart('Milk')">Add</button>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1585238342028-4c7c8d0a5c6b">
        <h3>Bread</h3>
        <p>₹35</p>
        <button onclick="addToCart('Bread')">Add</button>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1592928302636-c83cf1e1a2d6">
        <h3>Chips</h3>
        <p>₹20</p>
        <button onclick="addToCart('Chips')">Add</button>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1589927986089-35812388d1f4">
        <h3>Apples</h3>
        <p>₹120/kg</p>
        <button onclick="addToCart('Apples')">Add</button>
    </div>

    <div class="card">
        <img src="https://images.unsplash.com/photo-1604908176997-431f76c42a8c">
        <h3>Cold Drink</h3>
        <p>₹90</p>
        <button onclick="addToCart('Drink')">Add</button>
    </div>

</div>

<!-- YOUR NAME / PORTFOLIO -->
<section class="portfolio">
    <div class="profile">
        <img src="https://via.placeholder.com/150">
        <div>
            <h2>Dipika Sharma</h2>
            <p>B.Tech CSE Student | Future Developer 🚀</p>
        </div>
    </div>
</section>

<!-- FOOTER -->
<footer>
    <p>© 2026 Dipika Sharma | Blinkit Clone</p>
</footer>

<script>
function addToCart(item){
    alert(item + " added to cart 🛒");
}
</script>

</body>
</html>
