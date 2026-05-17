Got it! I added your contact info to the poster code. 

Bas ye file `index.html` ke naam se upload kar do GitHub pe, poster + contact details dono dikhenge:
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Deepika♡ Portfolio</title>
<style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Arial, sans-serif; }
    
    body {
        background: linear-gradient(135deg, #fff5f0 0%, #ffe8d6 100%);
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 20px;
    }
    
    .card {
        background: white;
        border-radius: 30px;
        padding: 50px 40px;
        max-width: 850px;
        width: 100%;
        box-shadow: 0 20px 60px rgba(255, 107, 53, 0.2);
        text-align: center;
    }
    
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 30px;
        flex-wrap: wrap;
        gap: 10px;
    }
    
    .logo {
        color: #ff6b35;
        font-weight: 700;
        font-size: 20px;
    }
    
    .tag {
        color: #666;
        font-size: 14px;
        background: #f5f5f5;
        padding: 6px 15px;
        border-radius: 20px;
    }
    
    h1 {
        color: #ff6b35;
        font-size: 48px;
        line-height: 1.2;
        margin: 20px 0;
        font-weight: 800;
    }
    
    h1 span {
        color: #3d3d3d;
        font-size: 36px;
        display: block;
    }
    
    .icons {
        font-size: 40px;
        margin: 20px 0;
    }
    
    .poster-img {
        width: 100%;
        max-width: 600px;
        border-radius: 20px;
        margin: 30px auto;
        display: block;
        box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    }
    
    .contact-box {
        background: #fff5f0;
        border-radius: 20px;
        padding: 25px;
        margin-top: 30px;
        text-align: left;
    }
    
    .contact-box h3 {
        color: #ff6b35;
        margin-bottom: 15px;
        font-size: 20px;
    }
    
    .contact-item {
        display: flex;
        align-items: center;
        gap: 12px;
        margin: 12px 0;
        color: #333;
        font-size: 16px;
    }
    
    .icon {
        width: 35px;
        height: 35px;
        background: #ff6b35;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-weight: bold;
        flex-shrink: 0;
    }
    
    .contact-item a {
        color: #ff6b35;
        text-decoration: none;
    }
    
    .contact-item a:hover {
        text-decoration: underline;
    }
    
    .btn {
        display: inline-block;
        padding: 15px 40px;
        background: #ff6b35;
        color: white;
        text-decoration: none;
        border-radius: 30px;
        font-weight: 600;
        font-size: 16px;
        margin-top: 25px;
        transition: all 0.3s ease;
    }
    
    .btn:hover {
        background: #e55a2b;
        transform: translateY(-3px);
        box-shadow: 0 10px 25px rgba(255, 107, 53, 0.3);
    }
    
    .footer {
        margin-top: 25px;
        color: #6a4c93;
        font-size: 16px;
        font-weight: 600;
    }
    
    @media (max-width: 600px) {
        h1 { font-size: 32px; }
        h1 span { font-size: 24px; }
        .card { padding: 30px 20px; }
    }
</style>
</head>
<body>
<div class="card">
    <div class="header">
        <div class="logo">♡ Deepika Sharma</div>
        <div class="tag">CS Student & Developer</div>
    </div>
    
    <div class="icons">💻 📱 🚀</div>
    
    <h1>Yeh se shuru<br><span>woh tak delivery</span></h1>
    
    <img src="https://i.ibb.co/8D3X9vQ/deepika-poster.png" alt="Deepika Portfolio" class="poster-img">
    
    <div class="footer">All my projects & links in one place</div>
    
    <a href="https://github.com/your-username" class="btn">View My GitHub</a>
    
    <div class="contact-box">
        <h3>Contact Me</h3>
        
        <div class="contact-item">
            <div class="icon">📞</div>
            <div>
                <strong>Phone:</strong> 
                <a href="tel:7440716313">7440716313</a>
            </div>
        </div>
        
        <div class="contact-item">
            <div class="icon">✉️</div>
            <div>
                <strong>Email:</strong> 
                <a href="mailto:deepikasharma8730@gmail.com">deepikasharma8730@gmail.com</a>
            </div>
        </div>
        
        <div class="contact-item">
            <div class="icon">📍</div>
            <div>
                <strong>Address:</strong> Bhopal
            </div>
        </div>
    </div>
</div>
</body>
</html>



