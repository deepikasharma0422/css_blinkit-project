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
        <div class="tag">India’s Last Minute App</div>

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

<!-- YOUR NAME -->
<div class="name">Made by Dipika Sharma 💚</div>

<script>
function openApp() {
    window.open("https://blinkit.com", "_blank");
}
</script>

</body>
</html>
