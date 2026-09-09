# kulswamini-maching-centre-jents-and-ladies-telaring-material-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Kulswamini Machine Centre | Gents & Ladies Tailoring Material</title>

  <meta name="description"
        content="Kulswamini Machine Centre - Gents & Ladies Tailoring Material, Threads, Buttons, Zips, Needles, Machine Accessories and more.">

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&family=Playfair+Display:wght@600;700&display=swap"
        rel="stylesheet">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Poppins',sans-serif;
      background:#fffaf5;
      color:#27221e;
      line-height:1.6;
    }

    a{
      text-decoration:none;
      color:inherit;
    }

    img{
      width:100%;
      display:block;
    }

    /* NAVBAR */

    header{
      position:fixed;
      top:0;
      left:0;
      width:100%;
      z-index:1000;
      background:rgba(255,255,255,0.96);
      box-shadow:0 3px 20px rgba(0,0,0,0.08);
    }

    nav{
      max-width:1200px;
      margin:auto;
      padding:15px 20px;
      display:flex;
      align-items:center;
      justify-content:space-between;
    }

    .logo{
      font-family:'Playfair Display',serif;
      font-size:25px;
      font-weight:700;
      color:#8b4a28;
    }

    .logo span{
      display:block;
      font-family:'Poppins',sans-serif;
      font-size:10px;
      letter-spacing:2px;
      color:#777;
      text-transform:uppercase;
    }

    .nav-links{
      display:flex;
      gap:25px;
      align-items:center;
    }

    .nav-links a{
      font-size:14px;
      font-weight:500;
      transition:.3s;
    }

    .nav-links a:hover{
      color:#b56535;
    }

    .nav-btn{
      background:#8b4a28;
      color:white !important;
      padding:10px 18px;
      border-radius:25px;
    }

    .menu{
      display:none;
      font-size:28px;
      cursor:pointer;
    }

    /* HERO */

    .hero{
      min-height:100vh;
      padding:130px 7% 70px;
      display:flex;
      align-items:center;
      background:
      linear-gradient(90deg,rgba(34,23,17,.9),rgba(34,23,17,.45)),
      url("https://images.unsplash.com/photo-1596462502278-27bfdc403348?auto=format&fit=crop&w=1800&q=80")
      center/cover;
      color:white;
    }

    .hero-content{
      max-width:700px;
    }

    .tag{
      display:inline-block;
      background:rgba(255,255,255,.15);
      border:1px solid rgba(255,255,255,.35);
      padding:8px 16px;
      border-radius:30px;
      font-size:13px;
      margin-bottom:20px;
    }

    .hero h1{
      font-family:'Playfair Display',serif;
      font-size:clamp(42px,6vw,76px);
      line-height:1.08;
      margin-bottom:20px;
    }

    .hero h1 span{
      color:#f2b37f;
    }

    .hero p{
      max-width:620px;
      color:#eee;
      font-size:17px;
      margin-bottom:30px;
    }

    .buttons{
      display:flex;
      gap:15px;
      flex-wrap:wrap;
    }

    .btn{
      display:inline-block;
      padding:13px 23px;
      border-radius:30px;
      font-weight:600;
      transition:.3s;
    }

    .btn-primary{
      background:#b56535;
      color:white;
    }

    .btn-primary:hover{
      background:#914923;
      transform:translateY(-2px);
    }

    .btn-light{
      border:1px solid white;
      color:white;
    }

    .btn-light:hover{
      background:white;
      color:#333;
    }

    /* COMMON */

    section{
      padding:85px 7%;
    }

    .section-title{
      text-align:center;
      margin-bottom:45px;
    }

    .section-title small{
      color:#b56535;
      font-weight:700;
      letter-spacing:2px;
      text-transform:uppercase;
    }

    .section-title h2{
      font-family:'Playfair Display',serif;
      font-size:42px;
      margin-top:8px;
    }

    .section-title p{
      color:#777;
      max-width:650px;
      margin:10px auto;
    }

    /* ABOUT */

    .about{
      max-width:1200px;
      margin:auto;
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:55px;
      align-items:center;
    }

    .about-img{
      border-radius:25px;
      overflow:hidden;
      box-shadow:0 20px 50px rgba(0,0,0,.12);
    }

    .about-img img{
      height:450px;
      object-fit:cover;
    }

    .about-text small{
      color:#b56535;
      font-weight:700;
      letter-spacing:2px;
    }

    .about-text h2{
      font-family:'Playfair Display',serif;
      font-size:42px;
      margin:10px 0 18px;
    }

    .about-text p{
      color:#666;
      margin-bottom:15px;
    }

    /* CATEGORIES */

    .category-grid{
      max-width:1200px;
      margin:auto;
      display:grid;
      grid-template-columns:repeat(4,1fr);
      gap:20px;
    }

    .category{
      background:white;
      padding:30px 20px;
      text-align:center;
      border-radius:20px;
      box-shadow:0 8px 30px rgba(0,0,0,.07);
      transition:.3s;
      border:1px solid #f0e4db;
    }

    .category:hover{
      transform:translateY(-8px);
      box-shadow:0 15px 35px rgba(0,0,0,.12);
    }

    .category .icon{
      width:70px;
      height:70px;
      margin:0 auto 18px;
      border-radius:50%;
      background:#f8e5d7;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:32px;
    }

    .category h3{
      font-size:18px;
      margin-bottom:7px;
    }

    .category p{
      color:#777;
      font-size:13px;
    }

    /* PRODUCTS */

    .products{
      background:#f7eee8;
    }

    .product-grid{
      max-width:1200px;
      margin:auto;
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:25px;
    }

    .product{
      background:white;
      border-radius:20px;
      overflow:hidden;
      box-shadow:0 8px 25px rgba(0,0,0,.08);
      transition:.3s;
    }

    .product:hover{
      transform:translateY(-7px);
    }

    .product img{
      height:220px;
      object-fit:cover;
    }

    .product-content{
      padding:22px;
    }

    .product-content h3{
      font-size:19px;
      margin-bottom:7px;
    }

    .product-content p{
      font-size:13px;
      color:#777;
      margin-bottom:15px;
    }

    .enquiry{
      display:inline-block;
      background:#8b4a28;
      color:white;
      padding:9px 17px;
      border-radius:20px;
      font-size:13px;
      font-weight:600;
    }

    /* WHY US */

    .why-grid{
      max-width:1100px;
      margin:auto;
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:25px;
    }

    .why{
      text-align:center;
      padding:30px 20px;
    }

    .why-icon{
      font-size:40px;
      margin-bottom:15px;
    }

    .why h3{
      margin-bottom:8px;
    }

    .why p{
      color:#777;
      font-size:14px;
    }

    /* GALLERY */

    .gallery{
      max-width:1200px;
      margin:auto;
      display:grid;
      grid-template-columns:repeat(4,1fr);
      gap:15px;
    }

    .gallery img{
      height:240px;
      object-fit:cover;
      border-radius:15px;
      transition:.3s;
    }

    .gallery img:hover{
      transform:scale(1.03);
    }

    /* CTA */

    .cta{
      margin:0 7% 80px;
      border-radius:30px;
      padding:65px 30px;
      text-align:center;
      color:white;
      background:
      linear-gradient(rgba(82,39,20,.88),rgba(82,39,20,.88)),
      url("https://images.unsplash.com/photo-1558618666-fcd25c85cd64?auto=format&fit=crop&w=1600&q=80")
      center/cover;
    }

    .cta h2{
      font-family:'Playfair Display',serif;
      font-size:42px;
      margin-bottom:12px;
    }

    .cta p{
      color:#eee;
      margin-bottom:25px;
    }

    /* CONTACT */

    .contact{
      max-width:1200px;
      margin:auto;
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:40px;
    }

    .contact-info{
      background:#f7eee8;
      padding:35px;
      border-radius:25px;
    }

    .contact-info h2{
      font-family:'Playfair Display',serif;
      font-size:35px;
      margin-bottom:20px;
    }

    .contact-item{
      display:flex;
      gap:15px;
      margin:20px 0;
      align-items:flex-start;
    }

    .contact-item .ci{
      font-size:23px;
    }

    .contact-item h4{
      font-size:14px;
      margin-bottom:2px;
    }

    .contact-item p{
      font-size:13px;
      color:#666;
    }

    .contact-form{
      background:white;
      padding:35px;
      border-radius:25px;
      box-shadow:0 8px 30px rgba(0,0,0,.07);
    }

    .contact-form h3{
      font-size:25px;
      margin-bottom:20px;
    }

    input,textarea,select{
      width:100%;
      padding:13px 15px;
      margin-bottom:15px;
      border:1px solid #ddd;
      border-radius:10px;
      outline:none;
      font-family:inherit;
      background:#fff;
    }

    textarea{
      height:120px;
      resize:none;
    }

    input:focus,textarea:focus,select:focus{
      border-color:#b56535;
    }

    .submit-btn{
      width:100%;
      border:none;
      cursor:pointer;
      background:#8b4a28;
      color:white;
      padding:14px;
      border-radius:10px;
      font-size:15px;
      font-weight:600;
    }

    /* FOOTER */

    footer{
      background:#241914;
      color:white;
      padding:45px 7% 20px;
    }

    .footer-grid{
      max-width:1200px;
      margin:auto;
      display:grid;
      grid-template-columns:2fr 1fr 1fr;
      gap:40px;
    }

    footer h2{
      font-family:'Playfair Display',serif;
      margin-bottom:10px;
    }

    footer p{
      color:#bbb;
      font-size:13px;
    }

    footer h4{
      margin-bottom:12px;
    }

    footer a{
      display:block;
      color:#bbb;
      font-size:13px;
      margin:7px 0;
    }

    footer a:hover{
      color:white;
    }

    .copyright{
      text-align:center;
      border-top:1px solid #493b34;
      margin-top:30px;
      padding-top:18px;
      color:#999;
      font-size:12px;
    }

    /* WHATSAPP */

    .whatsapp{
      position:fixed;
      right:20px;
      bottom:20px;
      width:58px;
      height:58px;
      background:#25D366;
      color:white;
      border-radius:50%;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:28px;
      box-shadow:0 5px 20px rgba(0,0,0,.2);
      z-index:999;
    }

    /* MOBILE */

    @media(max-width:900px){

      .nav-links{
        position:absolute;
        top:70px;
        right:20px;
        width:220px;
        background:white;
        padding:20px;
        border-radius:15px;
        box-shadow:0 10px 30px rgba(0,0,0,.15);
        display:none;
        flex-direction:column;
        align-items:stretch;
        gap:15px;
      }

      .nav-links.active{
        display:flex;
      }

      .menu{
        display:block;
      }

      .category-grid{
        grid-template-columns:repeat(2,1fr);
      }

      .product-grid{
        grid-template-columns:repeat(2,1fr);
      }

      .gallery{
        grid-template-columns:repeat(2,1fr);
      }

      .about,
      .contact{
        grid-template-columns:1fr;
      }

      .why-grid{
        grid-template-columns:1fr;
      }
    }

    @media(max-width:600px){

      section{
        padding:65px 5%;
      }

      .hero{
        padding:120px 6% 60px;
      }

      .hero h1{
        font-size:43px;
      }

      .hero p{
        font-size:14px;
      }

      .section-title h2,
      .about-text h2{
        font-size:34px;
      }

      .category-grid,
      .product-grid,
      .gallery{
        grid-template-columns:1fr;
      }

      .about-img img{
        height:330px;
      }

      .gallery img{
        height:250px;
      }

      .cta{
        margin:0 5% 60px;
        padding:45px 20px;
      }

      .cta h2{
        font-size:32px;
      }

      .footer-grid{
        grid-template-columns:1fr;
        gap:25px;
      }

    }

  </style>
</head>

<body>

<!-- NAVBAR -->

<header>
  <nav>

    <a href="#home" class="logo">
      Kulswamini
      <span>Machine Centre</span>
    </a>

    <div class="menu" onclick="toggleMenu()">☰</div>

    <div class="nav-links" id="navLinks">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#categories">Categories</a>
      <a href="#products">Products</a>
      <a href="#gallery">Gallery</a>
      <a href="#contact" class="nav-btn">Contact</a>
    </div>

  </nav>
</header>


<!-- HERO -->

<section class="hero" id="home">

  <div class="hero-content">

    <div class="tag">
      ✨ Gents & Ladies Tailoring Material
    </div>

    <h1>
      Everything You Need<br>
      For <span>Perfect Tailoring</span>
    </h1>

    <p>
      Quality tailoring material for gents and ladies —
      threads, buttons, zips, needles, machine accessories,
      measuring tools and much more.
    </p>

    <div class="buttons">

      <a href="#products" class="btn btn-primary">
        Explore Products
      </a>

      <a href="#contact" class="btn btn-light">
        Enquire Now
      </a>

    </div>

  </div>

</section>


<!-- ABOUT -->

<section id="about">

  <div class="about">

    <div class="about-img">
      <img
        src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?auto=format&fit=crop&w=1000&q=80"
        alt="Tailoring Material">
    </div>

    <div class="about-text">

      <small>ABOUT US</small>

      <h2>
        Kulswamini Machine Centre
      </h2>

      <p>
        Welcome to Kulswamini Machine Centre —
        your destination for gents and ladies tailoring material.
      </p>

      <p>
        We provide a wide range of tailoring essentials
        useful for tailors, boutiques, fashion designers
        and home sewing work.
      </p>

      <p>
        From everyday tailoring accessories to sewing machine
        essentials, you can enquire with us for the products
        you need.
      </p>

      <a href="#contact" class="btn btn-primary">
        Contact Us
      </a>

    </div>

  </div>

</section>


<!-- CATEGORIES -->

<section id="categories">

  <div class="section-title">

    <small>OUR CATEGORIES</small>

    <h2>
      Tailoring Essentials
    </h2>

    <p>
      Explore our main categories of tailoring materials.
    </p>

  </div>


  <div class="category-grid">

    <div class="category">
      <div class="icon">👔</div>
      <h3>Gents Material</h3>
      <p>
        Shirt, pant & suit tailoring accessories.
      </p>
    </div>


    <div class="category">
      <div class="icon">👗</div>
      <h3>Ladies Material</h3>
      <p>
        Blouse, dress & ladies tailoring accessories.
      </p>
    </div>


    <div class="category">
      <div class="icon">🧵</div>
      <h3>Threads & Needles</h3>
      <p>
        Different tailoring threads and needles.
      </p>
    </div>


    <div class="category">
      <div class="icon">✂️</div>
      <h3>Cutting Tools</h3>
      <p>
        Scissors, measuring tapes, chalk and tools.
      </p>
    </div>


    <div class="category">
      <div class="icon">🔘</div>
      <h3>Buttons</h3>
      <p>
        Different buttons for tailoring work.
      </p>
    </div>


    <div class="category">
      <div class="icon">〰️</div>
      <h3>Zips & Hooks</h3>
      <p>
        Zippers, hooks and other accessories.
      </p>
    </div>


    <div class="category">
      <div class="icon">⚙️</div>
      <h3>Machine Accessories</h3>
      <p>
        Sewing machine related accessories.
      </p>
    </div>


    <div class="category">
      <div class="icon">🎀</div>
      <h3>Laces & Piping</h3>
      <p>
        Decorative tailoring materials.
      </p>
    </div>

  </div>

</section>


<!-- PRODUCTS -->

<section class="products" id="products">

  <div class="section-title">

    <small>FEATURED MATERIAL</small>

    <h2>
      Popular Products
    </h2>

    <p>
      Product availability and pricing can be confirmed
      through WhatsApp enquiry.
    </p>

  </div>


  <div class="product-grid">


    <div class="product">

      <img
        src="https://images.unsplash.com/photo-1604881988758-f76ad2f7aac1?auto=format&fit=crop&w=900&q=80"
        alt="Tailoring Threads">

      <div class="product-content">

        <h3>Tailoring Threads</h3>

        <p>
          Quality threads for different tailoring requirements.
        </p>

        <a
          class="enquiry"
          href="https://wa.me/91XXXXXXXXXX?text=Hello%20Kulswamini%20Machine%20Centre,%20I%20want%20to%20enquire%20about%20Tailoring%20Threads."
          target="_blank">
          Enquire on WhatsApp
        </a>

      </div>

    </div>


    <div class="product">

      <img
        src="https://images.unsplash.com/photo-1594736797933-d0501ba2fe65?auto=format&fit=crop&w=900&q=80"
        alt="Buttons">

      <div class="product-content">

        <h3>Buttons Collection</h3>

        <p>
          Buttons suitable for gents and ladies garments.
        </p>

        <a
          class="enquiry"
          href="https://wa.me/91XXXXXXXXXX?text=Hello%20Kulswamini%20Machine%20Centre,%20I%20want%20to%20enquire%20about%20Buttons."
          target="_blank">
          Enquire on WhatsApp
        </a>

      </div>

    </div>


    <div class="product">

      <img
        src="https://images.unsplash.com/photo-1582738411706-bfc8e691d1c2?auto=format&fit=crop&w=900&q=80"
        alt="Sewing Accessories">

      <div class="product-content">

        <h3>Sewing Accessories</h3>

        <p>
          Useful accessories for sewing and tailoring work.
        </p>

        <a
          class="enquiry"
          href="https://wa.me/91XXXXXXXXXX?text=Hello%20Kulswamini%20Machine%20Centre,%20I%20want%20to%20enquire%20about%20Sewing%20Accessories."
          target="_blank">
          Enquire on WhatsApp
        </a>

      </div>

    </div>


    <div class="product">

      <img
        src="https://images.unsplash.com/photo-1595341888016-a392ef81b7de?auto=format&fit=crop&w=900&q=80"
        alt="Zippers">

      <div class="product-content">

        <h3>Zippers & Hooks</h3>

        <p>
          Zippers, hooks and other garment accessories.
        </p>

        <a
          class="enquiry"
          href="https://wa.me/91XXXXXXXXXX?text=Hello%20Kulswamini%20Machine%20Centre,%20I%20want%20to%20enquire%20about%20Zippers%20and%20Hooks."
          target="_blank">
          Enquire on WhatsApp
        </a>

      </div>

    </div>


    <div class="product">

      <img
        src="https://images.unsplash.com/photo-1610701596007-11502861dcfa?auto=format&fit=crop&w=900&q=80"
        alt="Measuring Tools">

      <div class="product-content">

        <h3>Measuring Tools</h3>

        <p>
          Measuring tapes, scales and tailoring tools.
        </p>

        <a
          class="enquiry"
          href="https://wa.me/91XXXXXXXXXX?text=Hello%20Kulswamini%20Machine%20Centre,%20I%20want%20to%20enquire%20about%20Measuring%20Tools."
          target="_blank">
          Enquire on WhatsApp
        </a>

      </div>

    </div>


    <div class="product">

      <img
        src="https://images.unsplash.com/photo-1598301257982-0cf014dabbcd?auto=format&fit=crop&w=900&q=80"
        alt="Ladies Tailoring Material">

      <div class="product-content">

        <h3>Ladies Tailoring Material</h3>

        <p>
          Blouse and ladies garment accessories.
        </p>

        <a
          class="enquiry"
          href="https://wa.me/91XXXXXXXXXX?text=Hello%20Kulswamini%20Machine%20Centre,%20I%20want%20to%20enquire%20about%20Ladies%20Tailoring%20Material."
          target="_blank">
          Enquire on WhatsApp
        </a>

      </div>

    </div>

  </div>

</section>


<!-- WHY US -->

<section>

  <div class="section-title">

    <small>WHY CHOOSE US</small>

    <h2>
  
