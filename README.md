# Yachana-art
YACHANA ART OFFICIAL WEBSITE 
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>YACHANA ART | Customized Acrylic & Blue Sign Boards</title>

  <meta name="description"
        content="YACHANA ART - Customized Acrylic Sign Boards, Blue Boards, Name Plates, Shop Boards and LED Sign Boards.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      color: #10233f;
      background: #ffffff;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
    }

    /* TOP BAR */
    .topbar {
      background: #062447;
      color: white;
      padding: 8px 5%;
      display: flex;
      justify-content: space-between;
      font-size: 14px;
    }

    /* HEADER */
    header {
      background: white;
      padding: 15px 5%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,.08);
    }

    .logo {
      font-size: 28px;
      font-weight: bold;
      color: #0b294d;
    }

    .logo span {
      color: #e6a900;
    }

    nav {
      display: flex;
      gap: 22px;
    }

    nav a {
      color: #10233f;
      font-weight: 600;
    }

    nav a:hover {
      color: #e6a900;
    }

    /* HERO */
    .hero {
      min-height: 570px;
      background:
        linear-gradient(90deg, rgba(3,27,52,.96), rgba(3,27,52,.72)),
        url("images/hero.jpg") center/cover;
      color: white;
      display: flex;
      align-items: center;
      padding: 60px 7%;
    }

    .hero-content {
      max-width: 650px;
    }

    .small-title {
      color: #f4bd26;
      font-size: 27px;
      font-style: italic;
      margin-bottom: 5px;
    }

    .hero h1 {
      font-size: clamp(40px, 6vw, 70px);
      line-height: 1.05;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 19px;
      margin-bottom: 28px;
    }

    .btn {
      display: inline-block;
      padding: 14px 25px;
      border-radius: 30px;
      font-weight: bold;
      margin: 5px;
      cursor: pointer;
    }

    .btn-gold {
      background: #f4bd26;
      color: #062447;
    }

    .btn-whatsapp {
      background: #19a947;
      color: white;
    }

    /* SECTION */
    section {
      padding: 70px 6%;
    }

    .section-title {
      text-align: center;
      margin-bottom: 40px;
    }

    .section-title h2 {
      font-size: 38px;
      color: #09284d;
    }

    .section-title p {
      color: #666;
    }

    /* PRODUCTS */
    .products {
      display: grid;
      grid-template-columns: repeat(6, 1fr);
      gap: 18px;
    }

    .product {
      border-radius: 12px;
      overflow: hidden;
      background: white;
      box-shadow: 0 4px 18px rgba(0,0,0,.12);
      transition: .3s;
    }

    .product:hover {
      transform: translateY(-5px);
    }

    .product img {
      width: 100%;
      height: 170px;
      object-fit: cover;
    }

    .product h3 {
      padding: 15px;
      font-size: 17px;
    }

    /* CUSTOMIZE */
    .customize {
      background: #f3f7fb;
    }

    .custom-box {
      max-width: 1100px;
      margin: auto;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 35px;
      align-items: center;
    }

    .form-box {
      background: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 5px 25px rgba(0,0,0,.08);
    }

    .form-box h2 {
      margin-bottom: 20px;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 13px;
      margin: 8px 0 16px;
      border: 1px solid #ddd;
      border-radius: 7px;
      font-size: 15px;
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    .custom-image img {
      width: 100%;
      border-radius: 15px;
    }

    /* GALLERY */
    .gallery {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 15px;
    }

    .gallery img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      border-radius: 10px;
    }

    /* WHY US */
    .features {
      display: grid;
      grid-template-columns: repeat(4,1fr);
      gap: 20px;
      text-align: center;
    }

    .feature {
      padding: 25px;
      border: 1px solid #eee;
      border-radius: 12px;
    }

    .feature .icon {
      font-size: 40px;
      margin-bottom: 10px;
    }

    /* CTA */
    .cta {
      background: #062447;
      color: white;
      text-align: center;
    }

    .cta h2 {
      font-size: 38px;
      margin-bottom: 15px;
    }

    /* FOOTER */
    footer {
      background: #031a31;
      color: white;
      padding: 50px 6% 20px;
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 2fr 1fr 1fr;
      gap: 40px;
    }

    footer h3 {
      color: #f4bd26;
      margin-bottom: 15px;
    }

    footer a {
      color: white;
      display: block;
      margin: 7px 0;
    }

    .copyright {
      text-align: center;
      border-top: 1px solid #29415c;
      margin-top: 30px;
      padding-top: 20px;
      font-size: 14px;
    }

    /* MOBILE */
    @media(max-width: 900px) {

      nav {
        display: none;
      }

      .products {
        grid-template-columns: repeat(2,1fr);
      }

      .custom-box {
        grid-template-columns: 1fr;
      }

      .gallery {
        grid-template-columns: repeat(2,1fr);
      }

      .features {
        grid-template-columns: repeat(2,1fr);
      }

      .topbar {
        font-size: 11px;
      }
    }

    @media(max-width: 550px) {

      .hero {
        min-height: 520px;
        padding: 40px 6%;
      }

      .hero h1 {
        font-size: 40px;
      }

      .products {
        grid-template-columns: 1fr 1fr;
      }

      .gallery {
        grid-template-columns: 1fr 1fr;
      }

      .features {
        grid-template-columns: 1fr;
      }

      section {
        padding: 50px 5%;
      }
    }
  </style>
</head>

<body>

<!-- TOP BAR -->
<div class="topbar">
  <div>📞 +91 XXXXXXXXXX | 💬 WhatsApp</div>
  <div>Customized Design | Premium Quality | On Time Delivery</div>
</div>


<!-- HEADER -->
<header>

  <div class="logo">
    YA <span>YACHANA ART</span>
  </div>

  <nav>
    <a href="#home">Home</a>
    <a href="#products">Our Designs</a>
    <a href="#customize">Customize</a>
    <a href="#gallery">Gallery</a>
    <a href="#about">About Us</a>
    <a href="#contact">Contact</a>
  </nav>

</header>


<!-- HERO -->
<section class="hero" id="home">

  <div class="hero-content">

    <div class="small-title">Customized</div>

    <h1>
      Acrylic Sign Boards
      & Blue Boards
    </h1>

    <p>
      आपके नाम, आपके डिजाइन और आपकी पहचान के लिए
      Premium Customized Sign Boards.
    </p>

    <a href="#customize" class="btn btn-gold">
      ✏️ Design Your Board
    </a>

    <a
      href="https://wa.me/91XXXXXXXXXX"
      class="btn btn-whatsapp"
      target="_blank">
      💬 Order on WhatsApp
    </a>

  </div>

</section>


<!-- PRODUCTS -->
<section id="products">

  <div class="section-title">
    <h2>Our Products</h2>
    <p>Choose Your Sign Board Category</p>
  </div>

  <div class="products">

    <div class="product">
      <img src="images/blue-board.jpg">
      <h3>🔵 Blue Boards</h3>
    </div>

    <div class="product">
      <img src="images/acrylic.jpg">
      <h3>✨ Acrylic Name Plate</h3>
    </div>

    <div class="product">
      <img src="images/shop-board.jpg">
      <h3>🏪 Shop Sign Board</h3>
    </div>

    <div class="product">
      <img src="images/office.jpg">
      <h3>🏢 Office Name Plate</h3>
    </div>

    <div class="product">
      <img src="images/led.jpg">
      <h3>💡 LED Sign Board</h3>
    </div>

    <div class="product">
      <img src="images/custom.jpg">
      <h3>🎨 Fully Customized</h3>
    </div>

  </div>

</section>


<!-- CUSTOMIZE -->
<section class="customize" id="customize">

  <div class="section-title">
    <h2>Customize Your Board</h2>
    <p>अपनी जरूरत बताइए और हम आपको best quotation देंगे।</p>
  </div>

  <div class="custom-box">

    <div class="form-box">

      <h2>Design Enquiry</h2>

      <form id="orderForm">

        <label>Name / Text *</label>
        <input
          type="text"
          id="name"
          placeholder="अपना नाम या Text लिखें"
          required>

        <label>Board Type *</label>

        <select id="board">
          <option>Blue Board</option>
          <option>Acrylic Name Plate</option>
          <option>Shop Sign Board</option>
          <option>Office Name Plate</option>
          <option>LED Sign Board</option>
          <option>Fully Customized</option>
        </select>

        <label>Size</label>

        <input
          type="text"
          id="size"
          placeholder="Example: 12 x 6 inch">

        <label>Background Color</label>

        <select id="background">
          <option>Blue</option>
          <option>Black</option>
          <option>White</option>
          <option>Transparent</option>
          <option>Other</option>
        </select>

        <label>Text Color</label>

        <select id="textcolor">
          <option>White</option>
          <option>Golden</option>
          <option>Black</option>
          <option>Other</option>
        </select>

        <label>Special Requirement</label>

        <textarea
          id="message"
          placeholder="अपनी जरूरत लिखें..."></textarea>

        <button
          type="submit"
          class="btn btn-whatsapp"
          style="border:0;width:100%;font-size:16px;">
          💬 Get Price / Order on WhatsApp
        </button>

      </form>

    </div>


    <div class="custom-image">

      <img src="images/custom-example.jpg"
           alt="Yachana Art Customized Sign Board">

    </div>

  </div>

</section>


<!-- GALLERY -->
<section id="gallery">

  <div class="section-title">
    <h2>Our Latest Work</h2>
    <p>Real Designs • Real Customers</p>
  </div>

  <div class="gallery">

    <img src="images/work1.jpg">
    <img src="images/work2.jpg">
    <img src="images/work3.jpg">
    <img src="images/work4.jpg">
    <img src="images/work5.jpg">
    <img src="images/work6.jpg">
    <img src="images/work7.jpg">
    <img src="images/work8.jpg">

  </div>

</section>


<!-- FEATURES -->
<section>

  <div class="section-title">
    <h2>Why Choose YACHANA ART?</h2>
  </div>

  <div class="features">

    <div class="feature">
      <div class="icon">✏️</div>
      <h3>100% Custom Design</h3>
      <p>Your idea, your creation.</p>
    </div>

    <div class="feature">
      <div class="icon">💎</div>
      <h3>Premium Quality</h3>
      <p>Long lasting & durable.</p>
    </div>

    <div class="feature">
      <div class="icon">🚚</div>
      <h3>Fast Delivery</h3>
      <p>On time delivery.</p>
    </div>

    <div class="feature">
      <div class="icon">🛡️</div>
      <h3>Safe Packaging</h3>
      <p>Secure packaging.</p>
    </div>

  </div>

</section>


<!-- CTA -->
<section class="cta" id="contact">

  <h2>अपने लिए Customized Board बनवाएँ</h2>

  <p>
    अपना नाम और डिजाइन हमें WhatsApp पर भेजें।
  </p>

  <br>

  <a
    href="https://wa.me/91XXXXXXXXXX"
    target="_blank"
    class="btn btn-whatsapp">

    💬 Chat on WhatsApp

  </a>

</section>


<!-- FOOTER -->
<footer id="about">

  <div class="footer-grid">

    <div>

      <h3>YACHANA ART</h3>

      <p>
        हम Customized Acrylic Sign Boards,
        Blue Boards, Name Plates, Shop Boards
        और अन्य customized signage बनाते हैं।
      </p>

    </div>


    <div>

      <h3>Quick Links</h3>

      <a href="#home">Home</a>
      <a href="#products">Our Designs</a>
      <a href="#customize">Customize</a>
      <a href="#gallery">Gallery</a>
      <a href="#contact">Contact</a>

    </div>


    <div>

      <h3>Contact Us</h3>

      <p>📞 +91 XXXXXXXXXX</p>

      <p>💬 WhatsApp Available</p>

      <p>📍 Your City, India</p>

    </div>

  </div>


  <div class="copyright">
    © 2026 YACHANA ART. All Rights Reserved.
  </div>

</footer>


<script>

  /* WhatsApp Order */

  document.getElementById("orderForm")
    .addEventListener("submit", function(e) {

      e.preventDefault();

      const name =
        document.getElementById("name").value;

      const board =
        document.getElementById("board").value;

      const size =
        document.getElementById("size").value;

      const background =
        document.getElementById("background").value;

      const textcolor =
        document.getElementById("textcolor").value;

      const message =
        document.getElementById("message").value;


      const phone = "9893963974";


      const whatsappMessage =
`नमस्ते YACHANA ART 👋

मुझे Customized Sign Board बनवाना है।

Name / Text: ${name}

Board Type: ${board}

Size: ${size}

Background Color: ${background}

Text Color: ${textcolor}

Special Requirement:
${message}

कृपया इसका Price बताएं।`;


      const url =
        "https://wa.me/" +
        phone +
        "?text=" +
        encodeURIComponent(whatsappMessage);


      window.open(url, "_blank");

  });

</script>

</body>
</html>
