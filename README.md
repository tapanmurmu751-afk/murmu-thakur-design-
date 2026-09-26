# murmu-thakur-design-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MURMU THAKUR DESIGN</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:Arial,sans-serif;background:#0b0b12;color:#fff;line-height:1.5}
header{padding:18px 6%;display:flex;justify-content:space-between;align-items:center;background:#11111b;position:sticky;top:0;z-index:10}
.logo{font-size:21px;font-weight:800;color:#ffd43b}
nav a{color:#fff;text-decoration:none;margin-left:18px;font-size:14px}
.hero{text-align:center;padding:75px 20px;background:linear-gradient(135deg,#17172a,#25103b)}
.hero h1{font-size:42px;margin-bottom:12px}
.hero p{color:#ddd;margin-bottom:25px}
.btn{display:inline-block;background:#25d366;color:#07110a;padding:13px 22px;border-radius:30px;text-decoration:none;font-weight:700}
section{padding:55px 6%}
.title{text-align:center;font-size:30px;margin-bottom:30px}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:18px}
.card{background:#171722;border:1px solid #292938;border-radius:16px;padding:22px;text-align:center}
.card .icon{font-size:42px;margin-bottom:10px}
.card h3{margin-bottom:7px}
.card p{color:#bbb;font-size:14px}
.price{color:#ffd43b;font-size:20px;font-weight:700;margin:12px 0}
form{max-width:650px;margin:auto;background:#171722;padding:25px;border-radius:18px}
input,textarea,select{width:100%;padding:13px;margin:8px 0 14px;border:1px solid #383849;border-radius:10px;background:#0e0e16;color:#fff}
button{width:100%;border:0;padding:14px;border-radius:10px;background:#25d366;font-weight:800;font-size:16px;cursor:pointer}
footer{text-align:center;padding:30px;background:#11111b;color:#aaa}
@media(max-width:650px){nav{display:none}.hero h1{font-size:31px}}
</style>
</head>
<body>
<header>
  <div class="logo">MURMU THAKUR DESIGN</div>
  <nav><a href="#services">Services</a><a href="#pricing">Pricing</a><a href="#order">Order</a></nav>
</header>

<section class="hero">
  <h1>Creative Posters. Powerful Designs.</h1>
  <p>Custom poster designs for events, businesses, birthdays, tournaments & more.</p>
  <a class="btn" href="https://wa.me/918984116800?text=Hello%20MURMU%20THAKUR%20DESIGN,%20I%20want%20a%20poster%20design." target="_blank">📲 Order on WhatsApp</a>
</section>

<section id="services">
<h2 class="title">Our Designs</h2>
<div class="cards">
  <div class="card"><div class="icon">🏆</div><h3>Tournament Posters</h3><p>Football, cricket, e-football and gaming events.</p></div>
  <div class="card"><div class="icon">🎂</div><h3>Birthday Posters</h3><p>Stylish birthday and celebration designs.</p></div>
  <div class="card"><div class="icon">💍</div><h3>Wedding Posters</h3><p>Wedding, invitation and special-event designs.</p></div>
  <div class="card"><div class="icon">📢</div><h3>Business Ads</h3><p>Promotional posters for shops and businesses.</p></div>
</div>
</section>

<section id="pricing">
<h2 class="title">Simple Pricing</h2>
<div class="cards">
  <div class="card"><h3>Basic Poster</h3><div class="price">₹99+</div><p>Simple social media poster.</p></div>
  <div class="card"><h3>Premium Poster</h3><div class="price">₹199+</div><p>Advanced creative design.</p></div>
  <div class="card"><h3>Custom Design</h3><div class="price">Ask Us</div><p>Price depends on your requirements.</p></div>
</div>
</section>

<section id="order">
<h2 class="title">Place Your Order</h2>
<form onsubmit="sendOrder(event)">
  <label>Your Name</label>
  <input id="name" required placeholder="Enter your name">
  <label>Poster Type</label>
  <select id="type">
    <option>Tournament Poster</option><option>Birthday Poster</option><option>Wedding Poster</option><option>Business Advertisement</option><option>Other</option>
  </select>
  <label>Details</label>
  <textarea id="details" rows="5" required placeholder="Tell us what you want on the poster"></textarea>
  <button type="submit">Send Order on WhatsApp</button>
</form>
</section>

<footer>
  <p>© 2026 MURMU THAKUR DESIGN</p>
  <p>WhatsApp: 8984116800</p>
</footer>

<script>
function sendOrder(e){
  e.preventDefault();
  const name=document.getElementById('name').value;
  const type=document.getElementById('type').value;
  const details=document.getElementById('details').value;
  const msg=`Hello MURMU THAKUR DESIGN!%0A%0AName: ${encodeURIComponent(name)}%0APoster Type: ${encodeURIComponent(type)}%0ADetails: ${encodeURIComponent(details)}`;
  window.open(`https://wa.me/918984116800?text=${msg}`,'_blank');
}
</script>
</body>
</html>