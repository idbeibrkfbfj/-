<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shoaib Topup</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .header {
            background: linear-gradient(135deg, #4a90e2, #145374);
            padding: 20px;
            text-align: center;
            position: relative;
        }
        .header img {
            width: 120px;
            height: auto;
            margin-bottom: 10px;
        }
        .header h1 {
            font-size: 40px;
            font-weight: bold;
            text-transform: uppercase;
            color: #fdfdfd;
            text-shadow: 2px 2px 4px #003366;
            letter-spacing: 3px;
            margin: 0;
        }
        .notice {
            background-color: #145374;
            color: white;
            padding: 10px;
            text-align: center;
            font-size: 16px;
            font-weight: bold;
            margin-bottom: 20px;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 15px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .options {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .option {
            flex: 1 1 calc(50% - 10px);
            background-color: #f9f9f9;
            margin: 5px;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            text-align: center;
            cursor: pointer;
        }
        .option span {
            font-weight: bold;
            display: block;
            margin-bottom: 5px;
        }
        .option .price {
            color: #145374;
            font-size: 16px;
        }
        .option.active {
            background-color: #ff9933;
            color: white;
            border-color: #cc7700;
        }
        .footer {
            background-color: #145374;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
        }
        .payment-methods {
            margin-top: 30px;
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .payment-options {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        .wallet-pay, .instant-pay {
            text-align: center;
            cursor: pointer;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 8px;
            background-color: #f9f9f9;
            max-width: 180px;
            position: relative;
        }
        .image-wrapper {
            width: 100px;
            height: 100px;
            margin: 0 auto;
            position: relative;
        }
        .wallet-pay img, .instant-pay img {
            width: 100%;
            height: 100%;
            border-radius: 12px;
            border: 2px solid #0000ff;
            box-shadow: 0 4px 8px rgba(0, 0, 255, 0.3);
        }
        .instant-pay.active, .wallet-pay.active {
            border-color: #ff9933;
            background-color: #ffe6cc;
        }
        .info-text {
            margin-top: 20px;
            font-size: 16px;
            font-weight: bold;
            color: #333;
        }
        .buy-now-btn {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
            font-weight: bold;
            color: #fff;
            background-color: #ff9933;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .buy-now-btn:hover {
            background-color: #cc7a29;
        }
    </style>
</head>
<body>
    <div class="header">
        <img src="https://i.ibb.co/hYv0rXk/yourimage.jpg" alt="Logo">
        <h1>Shoaib Topup</h1>
    </div>
    <div class="notice">
        <span>Instant Topup Service! Secure and Fast Transactions for All Users.</span>
    </div>
    <div class="container">
        <h2>Free Fire Topup</h2>
        <div class="options">
            <div class="option" onclick="selectOption(this, 25)">
                <span>25 Diamond</span>
                <span class="price">25 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 45)">
                <span>50 Diamond</span>
                <span class="price">45 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 90)">
                <span>115 Diamond</span>
                <span class="price">90 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 175)">
                <span>240 Diamond</span>
                <span class="price">175 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 245)">
                <span>355 Diamond</span>
                <span class="price">245 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 322)">
                <span>480 Diamond</span>
                <span class="price">322 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 390)">
                <span>505 Diamond</span>
                <span class="price">390 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 425)">
                <span>610 Diamond</span>
                <span class="price">425 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 610)">
                <span>850 Diamond</span>
                <span class="price">610 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 800)">
                <span>1090 Diamond</span>
                <span class="price">800 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 890)">
                <span>1240 Diamond</span>
                <span class="price">890 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 1662)">
                <span>2530 Diamond</span>
                <span class="price">1662 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 3999)">
                <span>5060 Diamond</span>
                <span class="price">3999 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 6999)">
                <span>10120 Diamond</span>
                <span class="price">6999 TK</span>
            </div>
            <!-- New Options -->
            <div class="option" onclick="selectOption(this, 180)">
                <span>Weekly</span>
                <span class="price">180 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 800)">
                <span>Monthly</span>
                <span class="price">800 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 180)">
                <span>Level Up Pass</span>
                <span class="price">180 TK</span>
            </div>
            <div class="option" onclick="selectOption(this, 50)">
                <span>Weekly Lite</span>
                <span class="price">50 TK</span>
            </div>
        </div>
    </div>
<div class="player-id" style="margin: 20px 0; text-align: center;">
    <label for="playerId" style="font-weight: bold; font-size: 18px; color: #145374; display: block; margin-bottom: 10px;">Player ID</label>
    <div style="position: relative; max-width: 400px; margin: 0 auto;">
        <input type="text" id="playerId" placeholder="Enter your Player ID (UID)" 
            style="
                width: 80%; /* কমানো হয়েছে */
                padding: 10px 15px; /* কমানো হয়েছে */
                font-size: 14px; /* কমানো হয়েছে */
                border: 2px solid transparent;
                border-radius: 25px;
                background: linear-gradient(white, white) padding-box, linear-gradient(90deg, red, orange, yellow, green, blue, indigo, violet) border-box;
                box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
                outline: none;
                text-align: center;
                animation: glow 2s infinite;
            ">
    </div>
</div>
    <div class="payment-methods">
        <h3>Select Payment Method</h3>
        <div class="payment-options">
            <div class="wallet-pay" onclick="selectPayment(this)">
                <div class="image-wrapper">
                    <img src="https://i.ibb.co/zbtP1N3/yourimage.jpg" alt="Wallet">
                </div>
                <p>Wallet Pay</p>
            </div>
            <div class="instant-pay active" onclick="selectPayment(this)">
                <div class="image-wrapper">
                    <img src="https://i.ibb.co/m9g01Vf/yourimage.jpg" alt="Instant Pay">
                </div>
                <p>Instant Pay</p>
            </div>
        </div>
        <p class="info-text">➡️ আপনার টাকা প্রয়োজন ৳ <span id="amountSelected">0</span></p>
        <button class="buy-now-btn">BUY NOW</button>
    </div>

    <div class="footer">
        &copy; 2024 Shoaib Topup. All rights reserved.
    </div>

    <script>
        function selectOption(element, price) {
            const options = document.querySelectorAll('.option');
            options.forEach(option => option.classList.remove('active'));
            element.classList.add('active');

            // Update the displayed price in the payment section
            document.getElementById('amountSelected').innerText = price;
        }

        function selectPayment(element) {
            const payments = document.querySelectorAll('.wallet-pay, .instant-pay');
            payments.forEach(payment => payment.classList.remove('active'));
            element.classList.add('active');
        }
    </script>
</body>
</html>
