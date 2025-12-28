<!DOCTYPE html>
<html lang="mg">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HARENA SHOP | Tsena an-tserasera</title>

<meta name="description" content="HARENA SHOP – fivarotana an-tserasera Malagasy mora sy azo antoka.">
<meta name="keywords" content="shop an-tserasera Malagasy, fivarotana en ligne, mividy an-tserasera">

<style>
body {margin:0;font-family:Arial;background:#f4f6f8;color:#333;}
header{background:#0d6efd;color:#fff;padding:20px;text-align:center;}
nav a{color:#fff;margin:0 8px;text-decoration:none;font-weight:bold;}
nav a:hover{text-decoration:underline;}
section{background:#fff;margin:20px;padding:25px;border-radius:10px;}
h2{color:#0d6efd;}
.hero{text-align:center;}
.hero button{margin:10px;padding:10px 20px;}
.products{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:15px;}
.product{border:1px solid #ddd;padding:15px;border-radius:10px;text-align:center;background:#fafafa;}
.product img{width:100%;height:180px;object-fit:cover;border-radius:8px;}
button{background:#0d6efd;color:#fff;border:none;padding:10px 15px;border-radius:5px;cursor:pointer;}
button:hover{background:#084298;}
.cart{background:#f1f1f1;padding:15px;border-radius:10px;}
footer{background:#222;color:#fff;text-align:center;padding:15px;}
.whatsapp{position:fixed;bottom:20px;right:20px;background:#25D366;color:#fff;padding:15px;border-radius:50%;font-size:22px;text-decoration:none;}
.admin{background:#eef;border:1px dashed #0d6efd;padding:15px;border-radius:10px;}
input,textarea{width:100%;padding:8px;margin:5px 0;border-radius:5px;border:1px solid #ccc;}
</style>
</head>

<body>

<header>
<h1>HARENA SHOP</h1>
<p>Tsena an-tserasera mora sy azo antoka ho an’ny rehetra</p>
<nav>
<a href="#home">Home</a>
<a href="#shop">Shop</a>
<a href="#checkout">Panier</a>
<a href="#about">About</a>
<a href="#delivery">Livraison</a>
<a href="#contact">Contact</a>
<a href="#admin">Admin</a>
</nav>
</header>

<section id="home" class="hero">
<h2>Tongasoa eto amin’ny HARENA SHOP</h2>
<p>Mividy mora, haingana ary azo antoka – eny rehetra eny.</p>
<button onclick="location.href='#shop'">Hividy izao</button>
<button onclick="sendWhatsApp()">Mifandray aminay amin’ny WhatsApp</button>
<ul>
<li>Vokatra tsara kalitao</li>
<li>Vidiny mirary</li>
<li>Livraison manerana an’i Madagasikara</li>
</ul>
</section>

<section id="shop">
<h2>Vokatra</h2>
<div class="products">
<div class="product">
<img src="https://images.unsplash.com/photo-1618354692139-9e31fcac3c0c?auto=format&fit=crop&w=400&q=80" alt="Akanjo">
<h3>Akanjo</h3><p>30 000 Ar</p>
<button onclick="addToCart('Akanjo',30000)">Ampidiro ao anaty panier</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1585386959984-a4155222db08?auto=format&fit=crop&w=400&q=80" alt="Kiraro">
<h3>Kiraro</h3><p>45 000 Ar</p>
<button onclick="addToCart('Kiraro',45000)">Ampidiro ao anaty panier</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1600180758890-64ec5038b7a5?auto=format&fit=crop&w=400&q=80" alt="Kitapo">
<h3>Kitapo</h3><p>35 000 Ar</p>
<button onclick="addToCart('Kitapo',35000)">Ampidiro ao anaty panier</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1580927752452-1d76e2a3c2d5?auto=format&fit=crop&w=400&q=80" alt="Accessoires">
<h3>Accessoires</h3><p>15 000 Ar</p>
<button onclick="addToCart('Accessoires',15000)">Ampidiro ao anaty panier</button>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1587825140708-7f987e9f2675?auto=format&fit=crop&w=400&q=80" alt="Kojakoja finday">
<h3>Kojakoja finday</h3><p>10 000 Ar</p>
<button onclick="addToCart('Kojakoja finday',10000)">Ampidiro ao anaty panier</button>
</div>
</div>
</section>

<section id="checkout">
<h2>Panier & Commande</h2>
<div class="cart" id="cart">Tsy mbola misy vokatra</div>

<h3>Fampahalalana mpanjifa</h3>
<input id="clientName" placeholder="Anaranao">
<input id="clientAddress" placeholder="Adiresy">
<textarea id="clientNote" placeholder="Fanamarihana"></textarea>

<h3>Fomba fandoavana</h3>
<ul>
<li>Mvola</li>
<li>Orange Money</li>
<li>Airtel Money</li>
<li>Paiement à la livraison</li>
</ul>

<button onclick="orderWhatsApp()">Alefa ny commande (WhatsApp)</button>
</section>

<section id="about">
<h2>Momba anay</h2>
<p>HARENA SHOP dia fivarotana an-tserasera natsangana hanamora ny fividianana vokatra isan-karazany ho an’ny olona rehetra eto Madagasikara.</p>
</section>

<section id="delivery">
<h2>Fandefasana</h2>
<ul>
<li>Manerana an’i Madagasikara</li>
<li>Mifandray mialoha amin’ny mpanjifa</li>
<li>Haingana sy azo itokisana</li>
</ul>
</section>

<section id="contact">
<h2>Contact</h2>
<p>Email: <b>harenah785@gmail.com</b></p>
<p>Téléphone / WhatsApp: <b>034 07 910 61</b></p>
</section>

<section id="admin" class="admin">
<h2>Admin Panel (Concept)</h2>
<p>✔️ Ajout / suppression produit (backend no ilaina raha tena izy)</p>
<p>✔️ Consultation commande</p>
<p>✔️ Gestion prix</p>
</section>

<footer>
<p>© 2025 HARENA SHOP – Shop an-tserasera Malagasy</p>
</footer>

<a class="whatsapp" onclick="sendWhatsApp()">💬</a>

<script>
let cart=[];

function addToCart(name,price){
cart.push({name,price});
displayCart();
}

function displayCart(){
let c=document.getElementById("cart");
let total=0;
c.innerHTML="<h3>Vokatra:</h3>";
cart.forEach(i=>{c.innerHTML+=`${i.name} - ${i.price} Ar<br>`;total+=i.price;});
c.innerHTML+=`<b>Total: ${total} Ar</b>`;
}

function orderWhatsApp(){
let name=document.getElementById("clientName").value;
let addr=document.getElementById("clientAddress").value;
let note=document.getElementById("clientNote").value;
let msg="Salama HARENA SHOP,%0ACommande:%0A";
cart.forEach(i=>msg+=`${i.name} - ${i.price} Ar%0A`);
msg+=`Total: ${cart.reduce((s,i)=>s+i.price,0)} Ar%0A`;
msg+=`Anarana: ${name}%0AAdiresy: ${addr}%0AFanamarihana: ${note}`;
window.open("https://wa.me/261340791061?text="+msg);
}

function sendWhatsApp(){
window.open("https://wa.me/261340791061?text=Salama%20HARENA%20SHOP,%20te-hanao%20commande%20aho");
}
</script>

</body>
</html>
