<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Promo Page</title>
  <style>
    body {
      margin: 0;
      background-color: #000;
      color: #fff;
      font-family: Arial, sans-serif;
    }
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px;
    }
    .logo img {
      height: 40px;
      border-radius: 50%;
    }
    .language-switcher button {
      margin: 0 5px;
      background: #fff;
      color: #000;
      padding: 5px 10px;
      border: none;
      cursor: pointer;
    }
    .product-image {
      display: block;
      margin: 20px auto;
      max-width: 90%;
      border: 3px solid red;
      border-radius: 10px;
    }
    .product-info {
      text-align: center;
      margin: 20px;
    }
    .price {
      font-size: 26px;
      color: #0f0;
      margin: 10px 0;
    }
    .cta {
      animation: pulse 1s infinite;
      background: #f00;
      padding: 10px 20px;
      display: inline-block;
      border-radius: 20px;
      margin: 20px auto;
      color: #fff;
      text-decoration: none;
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }
    .social {
      position: fixed;
      bottom: 10px;
      width: 100%;
      display: flex;
      justify-content: center;
      gap: 15px;
    }
    .social a {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      background: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .frame-link {
      text-align: center;
      margin: 20px;
    }
    .frame-link a {
      display: inline-block;
      background: #222;
      color: #0ff;
      padding: 10px 15px;
      border-radius: 10px;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">
      <img src="https://i.postimg.cc/bvvYy1gZ/1748637873743.png" alt="Fallaowme Logo">
    </div>
    <div class="language-switcher">
      <button onclick="setLanguage('ar')">عرب</button>
      <button onclick="setLanguage('fr')">FR</button>
      <button onclick="setLanguage('en')">EN</button>
    </div>
  </header>

  <img src="https://i.postimg.cc/dtM02ksf/Screenshot-20250611-000353.jpg" class="product-image" alt="Product Image">

  <div class="product-info" id="text-block">
    <h1 data-en="Magnetic Fast Charger" data-fr="Chargeur Magnétique Rapide" data-ar="شاحن مغناطيسي سريع">Magnetic Fast Charger</h1>
    <p data-en="A powerful and convenient magnetic charger for all your devices." data-fr="Un chargeur magnétique puissant et pratique pour tous vos appareils." data-ar="شاحن مغناطيسي قوي ومريح لجميع أجهزتك.">
      A powerful and convenient magnetic charger for all your devices.
    </p>
    <div class="price">MAD 139.99</div>
    <a href="https://s.click.aliexpress.com/e/_oEvqIZG" class="cta" target="_blank">Hurry before it’s gone!</a>
  </div>

  <div class="frame-link">
    <a href="https://s.click.aliexpress.com/e/_oEvqIZG" target="_blank">🔗 Visit Product Page</a>
  </div>

  <div class="social">
    <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/733/733547.png" width="20"></a>
    <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" width="20"></a>
    <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/733/733590.png" width="20"></a>
  </div>

  <script>
    function setLanguage(lang) {
      document.querySelectorAll('[data-' + lang + ']').forEach(el => {
        el.textContent = el.getAttribute('data-' + lang);
      });
    }
  </script>
</body>
</html>
