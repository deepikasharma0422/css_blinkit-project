<!DOCTYPE html>
<html>
<head>
<title>Blinkit Poster Clone - Dipika Sharma</title>

<style>
body {
    margin: 0;
    font-family: Arial;
}

/* MAIN POSTER */
.poster {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: linear-gradient(to right, #f7d400, #f5c400);
    padding: 40px;
    height: 100vh;
}

/* LEFT TEXT */
.left {
    width: 50%;
}

.logo {
    font-size: 40px;
    font-weight: bold;
    color: black;
}

.tag {
    font-size: 14px;
    margin-bottom: 20px;
}

.big-text {
    font-size: 50px;
    font-weight: bold;
}

.green {
    color: green;
}

.sub {
    margin-top: 10px;
    font-size: 18px;
}

/* FEATURES */
.features {
    display: flex;
    gap: 20px;
    margin-top: 30px;
}

.box {
    background: green;
    color: white;
    padding: 15px;
    border-radius: 10px;
    font-size: 14px;
}

/* RIGHT SIDE */
.right {
    width: 40%;
    text-align: center;
}

.right img {
    width: 300px;
}

/* BUTTON */
button {
    margin-top: 20px;
    padding: 10px 20px;
    background: black;
    color: white;
    border: none;
    cursor: pointer;
}

/* FOOTER NAME */
.name {
    position: absolute;
    bottom: 10px;
    right: 20px;
    font-weight: bold;
}
</style>

</head>

<body>

<div class="poster">

    <!-- LEFT -->
    <div class="left">
        <div class="logo">blinkit</div>
        <div class=  >India’s Last Minute App</div>C:\Users\M S I\OneDrive\Desktop
        <div class="big-text">
            Groceries delivered in <span class="green">10 minutes</span>
        </div>

        <div class="sub">
            Everything you need, delivered in a blink ⚡
        </div>

        <div class="features">
            <div class="box">⚡ 10 min delivery</div>
            <div class="box">⭐ Best quality</div>
            <div class="box">💸 Great offers</div>
        </div>

        <button onclick="openApp()">Shop Now</button>
    </div>

    <!-- RIGHT (PRODUCT IMAGE) -->
    <div class="right">
        <img src="https://images.unsplash.com/photo-1604908176997-431f76c42a8c">
    </div>

</div>


<script>
function openApp() {
    window.open("https://blinkit.com", "_blank");
}
</script>

</body>
</html>
}
</style>

</head>

<body>

<header>
    <h2 onclick="showSection('home')">Blinkit</h2>
    <div class="cart" onclick="showCart()">🛒 (<span id="count">0</span>)</div>
</header>

<!-- HOME -->
<div id="home" class="section active">
    <div class="poster">
        <div>
            <div class="big-text">Groceries in 10 minutes ⚡</div>
            <button onclick="showSection('shop')">Shop Now</button>
        </div>
        <img src="https://images.unsplash.com/photo-1604908176997-431f76c42a8c" width="250">
    </div>
</div>

<!-- SHOP -->
<div id="shop" class="section">
    <h2>All Groceries</h2>

    <div class="grid">

        <!-- MANY PRODUCTS -->
        <script>
        let products = [
            {name:"Apple", price:120, img:"https://images.unsplash.com/photo-1589927986089-35812388d1f4"},
            {name:"Banana", price:40, img:"https://images.unsplash.com/photo-1567306226416-28f0efdc88ce"},
            {name:"Milk", price:50, img:"https://images.unsplash.com/photo-1582719478250-c89cae4dc85b"},
            {name:"Bread", price:30, img:"https://images.unsplash.com/photo-1608198093002-ad4e005484ec"},
            {name:"Eggs", price:80, img:"https://images.unsplash.com/photo-1518569656558-1f25e69d93d7"},
            {name:"Rice", price:200, img:"https://images.unsplash.com/photo-1586201375761-83865001e31c"},
            {name:"Oil", price:150, img:"https://images.unsplash.com/photo-1615484477201-9d3b3f9b49f6"},
            {name:"Chips", price:20, img:"https://images.unsplash.com/photo-1585238342028-4c7c8d0a5c6b"},
            {name:"Chocolate", price:60, img:"https://images.unsplash.com/photo-1606313564200-e75d5e30476c"},
            {name:"Juice", price:90, img:"https://images.unsplash.com/photo-1571689936114-b16146f0c3f5"},
            {name:"Tomato", price:40, img:"https://images.unsplash.com/photo-1567306226416-28f0efdc88ce"},
            {name:"Potato", price:30, img:"https://images.unsplash.com/photo-1582515073490-dc3b0c5cfd74"}
        ];

        let html="";
        products.forEach((p,i)=>{
            html+=`
            <div class="card">
                <img src="${p.img}">
                <p>${p.name}</p>
                <p>₹${p.price}</p>
                <button onclick="addToCart(${i})">Add</button>
                <button onclick="buyNow(${i})">Buy</button>
            </div>`;
        });
        document.write(html);
        </script>

    </div>
</div>

<!-- CART -->
<div id="cartPage" class="section">
    <h2>Your Cart</h2>
    <div id="cartItems"></div>
    <h3 id="total"></h3>
    <button onclick="checkout()">Proceed to Checkout</button>
</div>

<!-- CHECKOUT -->
<div id="checkoutPage" class="section">
    <h2>Checkout</h2>

    <div class="payment-box">
        <input placeholder="Full Name">
        <input placeholder="Address">
        <input placeholder="Phone Number">

        <h3>Select Payment</h3>

        <button onclick="pay('UPI')">UPI</button>
        <button onclick="pay('Card')">Card</button>
        <button onclick="pay('COD')">Cash on Delivery</button>
    </div>
</div>

<!-- ORDER SUCCESS -->
<div id="successPage" class="section">
    <h1>✅ Order Placed Successfully</h1>
    <p>Thank you Dipika Sharma 💚</p>
    <button onclick="showSection('home')">Go Home</button>
</div>

<script>
let cart=[];

/* NAVIGATION */
function showSection(id){
    document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'));
    document.getElementById(id).classList.add('active');
}

/* CART FUNCTIONS */
function addToCart(i){
    cart.push(products[i]);
    document.getElementById("count").innerText = cart.length;
    alert(products[i].name + " added");
}

function buyNow(i){
    cart.push(products[i]);
    showCart();
}

function showCart(){
    showSection('cartPage');
    let items="";
    let total=0;

    cart.forEach(p=>{
        items+=`<div class="cart-item">${p.name} - ₹${p.price}</div>`;
        total+=p.price;
    });

    document.getElementById("cartItems").innerHTML = items;
    document.getElementById("total").innerText = "Total: ₹" + total;
}

/* CHECKOUT */
function checkout(){
    showSection('checkoutPage');
}

/* PAYMENT */
function pay(method){
    alert("Payment via " + method + " successful ✅");
    cart=[];
    document.getElementById("count").innerText = 0;
    showSection('successPage');
}
</script>

</body>
</html>
<!-- YOUR NAME -->
<div class="name">Made by Dipika Sharma 💚</div>


