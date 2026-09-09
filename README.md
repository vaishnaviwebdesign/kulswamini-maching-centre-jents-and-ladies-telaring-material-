<!DOCTYPE html>
<html lang="mr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>कुलस्वामिनी मशीन सेंटर | टेलरिंग साहित्य</title>

  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Devanagari:wght@400;500;600;700;800&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Noto Sans Devanagari',sans-serif;
      background:#fffaf5;
      color:#2d2118;
      line-height:1.6;
    }

    a{
      text-decoration:none;
      color:inherit;
    }

    .navbar{
      position:fixed;
      top:0;
      width:100%;
      z-index:1000;
      background:rgba(255,255,255,.96);
      box-shadow:0 2px 15px rgba(0,0,0,.08);
    }

    .nav-container{
      max-width:1200px;
      margin:auto;
      padding:14px 20px;
      display:flex;
      justify-content:space-between;
      align-items:center;
    }

    .logo{
      font-size:22px;
      font-weight:800;
      color:#8b3a16;
    }

    .logo span{
      display:block;
      font-size:12px;
      color:#777;
      font-weight:500;
    }

    .nav-links{
      display:flex;
      gap:24px;
      list-style:none;
    }

    .nav-links a{
      font-size:14px;
      font-weight:600;
      transition:.3s;
    }

    .nav-links a:hover{
      color:#c25b20;
    }

    .hero{
      min-height:100vh;
      padding:130px 20px 70px;
      display:flex;
      align-items:center;
      background:
        linear-gradient(rgba(55,25,10,.72),rgba(55,25,10,.72)),
        url("https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?auto=format&fit=crop&w=1600&q=80");
      background-size:cover;
      background-position:center;
      color:white;
    }

    .hero-content{
      max-width:1150px;
      margin:auto;
      width:100%;
    }

    .hero h1{
      font-size:52px;
      max-width:750px;
      line-height:1.25;
      margin-bottom:20px;
    }

    .hero p{
      max-width:650px;
      font-size:19px;
      margin-bottom:30px;
      color:#f7eeee;
    }

    .buttons{
      display:flex;
      gap:15px;
      flex-wrap:wrap;
    }

    .btn{
      padding:13px 24px;
      border-radius:30px;
      font-weight:700;
      display:inline-block;
      transition:.3s;
    }

    .btn-primary{
      background:#e66b24;
      color:white;
    }

    .btn-primary:hover{
      background:#c95213;
      transform:translateY(-2px);
    }

    .btn-light{
      background:white;
      color:#8b3a16;
    }

    section{
      padding:80px 20px;
    }

    .container{
      max-width:1150px;
      margin:auto;
    }

    .section-title{
      text-align:center;
      margin-bottom:45px;
    }

    .section-title h2{
      font-size:34px;
      color:#7c3213;
      margin-bottom:8px;
    }

    .section-title p{
      color:#777;
    }

    .about{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:45px;
      align-items:center;
    }

    .about img{
      width:100%;
      height:400px;
      object-fit:cover;
      border-radius:20px;
      box-shadow:0 10px 30px rgba(0,0,0,.12);
    }

    .about-text h3{
      font-size:28px;
      margin-bottom:15px;
      color:#8b3a16;
    }

    .about-text p{
      color:#666;
      margin-bottom:15px;
    }

    .categories{
      background:#f8eee5;
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(4,1fr);
      gap:20px;
    }

    .card{
      background:white;
      border-radius:18px;
      padding:25px 18px;
      text-align:center;
      box-shadow:0 5px 20px rgba(0,0,0,.07);
      transition:.3s;
    }

    .card:hover{
      transform:translateY(-7px);
      box-shadow:0 12px 28px rgba(0,0,0,.12);
    }

    .icon{
      width:70px;
      height:70px;
      border-radius:50%;
      background:#fff0e5;
      display:flex;
      align-items:center;
      justify-content:center;
      margin:0 auto 15px;
      font-size:32px;
    }

    .card h3{
      font-size:18px;
      margin-bottom:7px;
      color:#6f2c12;
    }

    .card p{
      color:#777;
      font-size:14px;
    }

    .products{
      grid-template-columns:repeat(3,1fr);
    }

    .product{
      overflow:hidden;
      padding:0;
      text-align:left;
    }

    .product img{
      width:100%;
      height:210px;
      object-fit:cover;
    }

    .product-content{
      padding:20px;
    }

    .product-content h3{
      margin-bottom:7px;
    }

    .why{
      background:#fff;
    }

    .why-grid{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:25px;
    }

    .why-box{
      padding:30px;
      background:#fff8f2;
      border-radius:18px;
      border-left:4px solid #d96521;
    }

    .why-box h3{
      margin-bottom:8px;
      color:#7c3213;
    }

    .gallery{
      background:#f8eee5;
    }

    .gallery-grid{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:15px;
    }

    .gallery-grid img{
      width:100%;
      height:230px;
      object-fit:cover;
      border-radius:15px;
      transition:.3s;
    }

    .gallery-grid img:hover{
      transform:scale(1.03);
    }

    .cta{
      background:
        linear-gradient(rgba(100,42,15,.85),rgba(100,42,15,.85)),
        url("https://images.unsplash.com/photo-1558618666-fcd25c85cd64?auto=format&fit=crop&w=1600&q=80");
      background-size:cover;
      background-position:center;
      text-align:center;
      color:white;
    }

    .cta h2{
      font-size:38px;
      margin-bottom:12px;
    }

    .cta p{
      margin-bottom:25px;
    }

    .contact{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:35px;
    }

    .contact-box{
      background:white;
      padding:30px;
      border-radius:18px;
      box-shadow:0 5px 20px rgba(0,0,0,.07);
    }

    .contact-item{
      margin-bottom:22px;
    }

    .contact-item h3{
      color:#8b3a16;
      margin-bottom:4px;
    }

    form input,
    form textarea{
      width:100%;
      padding:13px;
      margin-bottom:14px;
      border:1px solid #ddd;
      border-radius:10px;
      font-family:inherit;
      outline:none;
    }

    form textarea{
      height:130px;
      resize:none;
    }

    form button{
      border:none;
      cursor:pointer;
      font-family:inherit;
      width:100%;
    }

    footer{
      background:#28170e;
      color:white;
      text-align:center;
      padding:25px 15px;
    }

    footer p{
      font-size:14px;
      color:#ddd;
    }

    .whatsapp{
      position:fixed;
      right:20px;
      bottom:20px;
      width:58px;
      height:58px;
      border-radius:50%;
      background:#25d366;
      color:white;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:27px;
      z-index:999;
      box-shadow:0 5px 18px rgba(0,0,0,.25);
    }

    @media(max-width:900px){
      .nav-links{
        display:none;
      }

      .hero h1{
        font-size:40px;
      }

      .grid{
        grid-template-columns:repeat(2,1fr);
      }

      .products{
        grid-template-columns:repeat(2,1fr);
      }

      .about,
      .contact{
        grid-template-columns:1fr;
      }

      .why-grid{
        grid-template-columns:1fr;
      }

      .gallery-grid{
        grid-template-columns:repeat(2,1fr);
      }
    }

    @media(max-width:600px){
      .hero{
        padding-top:120px;
      }

      .hero h1{
        font-size:32px;
      }

      .hero p{
        font-size:16px;
      }

      section{
        padding:60px 15px;
      }

      .grid,
      .products,
      .gallery-grid{
        grid-template-columns:1fr;
      }

      .section-title h2{
        font-size:28px;
      }

      .about img{
        height:280px;
      }
    }
  </style>
</head>

<body>

<!-- NAVBAR -->
<nav class="navbar">
  <div class="nav-container">

    <div class="logo">
      🧵 कुलस्वामिनी मशीन सेंटर
      <span>जेंट्स व लेडीज टेलरिंग साहित्य</span>
    </div>

    <ul class="nav-links">
      <li><a href="#home">मुख्यपृष्ठ</a></li>
      <li><a href="#about">आमच्याबद्दल</a></li>
      <li><a href="#categories">साहित्य</a></li>
      <li><a href="#products">उत्पादने</a></li>
      <li><a href="#gallery">गॅलरी</a></li>
      <li><a href="#contact">संपर्क</a></li>
    </ul>

  </div>
</nav>


<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-content">

    <h1>
      शिवणकामासाठी लागणारे
      सर्व साहित्य एकाच ठिकाणी
    </h1>

    <p>
      कुलस्वामिनी मशीन सेंटरमध्ये जेंट्स आणि लेडीज
      टेलरिंगसाठी आवश्यक विविध प्रकारचे साहित्य उपलब्ध.
    </p>

    <div class="buttons">
      <a href="#products" class="btn btn-primary">
        🛍️ साहित्य पहा
      </a>

      <a href="#contact" class="btn btn-light">
        📞 आमच्याशी संपर्क करा
      </a>
    </div>

  </div>
</section>


<!-- ABOUT -->
<section id="about">
  <div class="container">

    <div class="section-title">
      <h2>आमच्याबद्दल</h2>
      <p>कुलस्वामिनी मशीन सेंटर</p>
    </div>

    <div class="about">

      <img src="https://images.unsplash.com/photo-1556909212-d5b604d0c90d?auto=format&fit=crop&w=1000&q=80">

      <div class="about-text">

        <h3>आपल्या टेलरिंग व्यवसायासाठी योग्य साहित्य</h3>

        <p>
          कुलस्वामिनी मशीन सेंटरमध्ये जेंट्स व लेडीज
          टेलरिंगसाठी लागणारे विविध प्रकारचे साहित्य
          उपलब्ध करून दिले जाते.
        </p>

        <p>
          दोरे, सुया, बटणे, झिप, हुक, लेस, पायपिंग,
          कटिंग व मोजमाप साहित्य तसेच शिवण मशीनचे
          विविध साहित्य येथे मिळते.
        </p>

        <p>
          आपल्या गरजेनुसार योग्य साहित्य निवडण्यासाठी
          आमच्याशी संपर्क करा.
        </p>

      </div>

    </div>

  </div>
</section>


<!-- CATEGORIES -->
<section class="categories" id="categories">

  <div class="container">

    <div class="section-title">
      <h2>आमच्याकडे उपलब्ध साहित्य</h2>
      <p>टेलरिंगसाठी आवश्यक विविध प्रकारचे साहित्य</p>
    </div>

    <div class="grid">

      <div class="card">
        <div class="icon">👔</div>
        <h3>जेंट्स टेलरिंग साहित्य</h3>
        <p>शर्ट, पँट व इतर कपड्यांसाठी आवश्यक साहित्य.</p>
      </div>

      <div class="card">
        <div class="icon">👗</div>
        <h3>लेडीज टेलरिंग साहित्य</h3>
        <p>ड्रेस, ब्लाऊज व इतर कपड्यांसाठी साहित्य.</p>
      </div>

      <div class="card">
        <div class="icon">🧵</div>
        <h3>दोरे व सुया</h3>
        <p>विविध प्रकारचे दोरे आणि शिवणकामाच्या सुया.</p>
      </div>

      <div class="card">
        <div class="icon">📏</div>
        <h3>कटिंग व मोजमाप</h3>
        <p>मोजपट्टी, स्केल आणि कटिंगसाठी लागणारे साहित्य.</p>
      </div>

      <div class="card">
        <div class="icon">🔘</div>
        <h3>बटणे</h3>
        <p>विविध आकार व डिझाईनची बटणे.</p>
      </div>

      <div class="card">
        <div class="icon">🤐</div>
        <h3>झिप व हुक</h3>
        <p>कपड्यांसाठी विविध प्रकारच्या झिप व हुक.</p>
      </div>

      <div class="card">
        <div class="icon">⚙️</div>
        <h3>शिवण मशीन साहित्य</h3>
        <p>शिवण मशीनसाठी आवश्यक विविध साहित्य.</p>
      </div>

      <div class="card">
        <div class="icon">🎀</div>
        <h3>लेस व पायपिंग</h3>
        <p>ड्रेस व ब्लाऊजसाठी विविध लेस व पायपिंग.</p>
      </div>

    </div>

  </div>
</section>


<!-- PRODUCTS -->
<section id="products">

  <div class="container">

    <div class="section-title">
      <h2>लोकप्रिय साहित्य</h2>
      <p>आमच्याकडे मिळणाऱ्या काही वस्तू</p>
    </div>

    <div class="grid products">

      <div class="card product">
        <img src="https://images.unsplash.com/photo-1598733088498-0d3c2a7a0b5f?auto=format&fit=crop&w=900&q=80">

        <div class="product-content">
          <h3>🧵 टेलरिंग दोरे</h3>
          <p>विविध रंग व प्रकारातील शिवणकामाचे दोरे.</p>
        </div>
      </div>


      <div class="card product">
        <img src="https://images.unsplash.com/photo-1610701596007-11502861dcfa?auto=format&fit=crop&w=900&q=80">

        <div class="product-content">
          <h3>🔘 बटणे</h3>
          <p>जेंट्स व लेडीज कपड्यांसाठी विविध बटणे.</p>
        </div>
      </div>


      <div class="card product">
        <img src="https://images.unsplash.com/photo-1604881988758-f76ad2f7aac1?auto=format&fit=crop&w=900&q=80">

        <div class="product-content">
          <h3>🤐 झिप व हुक</h3>
          <p>विविध आकाराच्या झिप व हुक उपलब्ध.</p>
        </div>
      </div>


      <div class="card product">
        <img src="https://images.unsplash.com/photo-1583845112203-454c8b6d7c7c?auto=format&fit=crop&w=900&q=80">

        <div class="product-content">
          <h3>📏 मोजमाप साहित्य</h3>
          <p>टेलरिंगसाठी आवश्यक मोजपट्टी व इतर साहित्य.</p>
        </div>
      </div>


      <div class="card product">
        <img src="https://images.unsplash.com/photo-1598301257982-0cf014dabbcd?auto=format&fit=crop&w=900&q=80">

        <div class="product-content">
          <h3>⚙️ मशीन साहित्य</h3>
          <p>शिवण मशीनसाठी आवश्यक साहित्य व अॅक्सेसरीज.</p>
        </div>
      </div>


      <div class="card product">
        <img src="https://images.unsplash.com/photo-1591369822096-ffd140ec948f?auto=format&fit=crop&w=900&q=80">

        <div class="product-content">
          <h3>🎀 लेडीज टेलरिंग साहित्य</h3>
          <p>ब्लाऊज व ड्रेससाठी विविध प्रकारचे साहित्य.</p>
        </div>
      </div>

    </div>

  </div>
</section>


<!-- WHY CHOOSE US -->
<section class="why">

  <div class="container">

    <div class="section-title">
      <h2>आम्हाला का निवडावे?</h2>
      <p>ग्राहकांसाठी आमचे प्रयत्न</p>
    </div>

    <div class="why-grid">

      <div class="why-box">
        <h3>⭐ विविध प्रकारचे साहित्य</h3>
        <p>
          जेंट्स आणि लेडीज टेलरिंगसाठी
          विविध प्रकारचे साहित्य एकाच ठिकाणी.
        </p>
      </div>

      <div class="why-box">
        <h3>💯 चांगली गुणवत्ता</h3>
        <p>
          आपल्या शिवणकामासाठी उपयोगी आणि
          दर्जेदार साहित्य मिळवण्याचा प्रयत्न.
        </p>
      </div>

      <div class="why-box">
        <h3>🤝 ग्राहक सेवा</h3>
        <p>
          आपल्या गरजेनुसार साहित्य निवडण्यासाठी
          योग्य मार्गदर्शन.
        </p>
      </div>

    </div>

  </div>
</section>


<!-- GALLERY -->
<section class="gallery" id="gallery">

  <div class="container">

    <div class="section-title">
      <h2>उत्पादनांची गॅलरी</h2>
      <p>आमच्या दुकानातील साहित्याची झलक</p>
    </div>

    <div class="gallery-grid">

      <img src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?auto=format&fit=crop&w=900&q=80">

      <img src="https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?auto=format&fit=crop&w=900&q=80">

      <img src="https://images.unsplash.com/photo-1556909212-d5b604d0c90d?auto=format&fit=crop&w=900&q=80">

      <img src="https://images.unsplash.com/photo-1598301257982-0cf014dabbcd?auto=format&fit=crop&w=900&q=80">

      <img src="https://images.unsplash.com/photo-1583845112203-454c8b6d7c7c?auto=format&fit=crop&w=900&q=80">

      <img src="https://images.unsplash.com/photo-1591369822096-ffd140ec948f?auto=format&fit=crop&w=900&q=80">

    </div>

  </div>
</section>


<!-- CTA -->
<section class="cta">

  <div class="container">

    <h2>टेलरिंग साहित्य हवे आहे?</h2>

    <p>
      आजच आमच्याशी संपर्क करा आणि आपल्या गरजेचे साहित्य विचारा.
    </p>

    <a
      href="https://wa.me/91XXXXXXXXXX?text=नमस्कार,%20मला%20टेलरिंग%20साहित्याबद्दल%20माहिती%20हवी%20आहे."
      class="btn btn-primary">
      💬 WhatsApp वर चौकशी करा
    </a>

  </div>

</section>


<!-- CONTACT -->
<section id="contact">

  <div class="container">

    <div class="section-title">
      <h2>आमच्याशी संपर्क साधा</h2>
      <p>साहित्याबद्दल चौकशी करण्यासाठी संपर्क करा</p>
    </div>

    <div class="contact">

      <div class="contact-box">

        <div class="contact-item">
          <h3>📍 दुकानाचा पत्ता</h3>
          <p>आपला दुकानाचा पूर्ण पत्ता येथे टाका</p>
        </div>

        <div class="contact-item">
          <h3>📞 मोबाईल नंबर</h3>
          <p>+91 XXXXXXXXXX</p>
        </div>

        <div class="contact-item">
          <h3>💬 WhatsApp</h3>
          <p>टेलरिंग साहित्याबद्दल WhatsApp वर चौकशी करा.</p>
        </div>

        <div class="contact-item">
          <h3>🕐 दुकानाची वेळ</h3>
          <p>सोमवार ते रविवार — सकाळी 9 ते रात्री 9</p>
        </div>

      </div>


      <div class="contact-box">

        <h3 style="margin-bottom:18px;color:#8b3a16;">
          WhatsApp वर चौकशी करा
        </h3>

        <form onsubmit="sendWhatsApp(); return false;">

          <input
            type="text"
            id="name"
            placeholder="आपले नाव"
            required>

          <input
            type="text"
            id="product"
            placeholder="आपल्याला कोणते साहित्य हवे आहे?"
            required>

          <textarea
            id="message"
            placeholder="आपला संदेश"></textarea>

          <button class="btn btn-primary">
            WhatsApp वर संदेश पाठवा
          </button>

        </form>

      </div>

    </div>

  </div>

</section>


<!-- FOOTER -->
<footer>

  <p>
    © 2026 कुलस्वामिनी मशीन सेंटर. सर्व हक्क राखीव.
  </p>

  <p>
    जेंट्स व लेडीज टेलरिंग साहित्य
  </p>

</footer>


<!-- FLOATING WHATSAPP -->
<a
  class="whatsapp"
  href="https://wa.me/91XXXXXXXXXX?text=नमस्कार,%20मला%20टेलरिंग%20साहित्याबद्दल%20माहिती%20हवी%20आहे."
  target="_blank">
  💬
</a>


<script>

function sendWhatsApp(){

  let name = document.getElementById("name").value;
  let product = document.getElementById("product").value;
  let message = document.getElementById("message").value;

  let text =
  "नमस्कार कुलस्वामिनी मशीन सेंटर,%0A%0A" +
  "नाव: " + name + "%0A" +
  "साहित्य: " + product + "%0A" +
  "संदेश: " + message;

  let phone = "91XXXXXXXXXX";

  window.open(
    "https://wa.me/" + phone + "?text=" + text,
    "_blank"
  );
}

</script>

</body>
</html>
