<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>eFootball Account Market</title>

<style>
body{
margin:0;
font-family:Arial;
background:linear-gradient(135deg,#001f3f,#003366);
color:white;
}

header{
background:#0a1f44;
padding:20px;
text-align:center;
border-bottom:3px solid #f7ff00;
}

header h1{
margin:0;
color:#f7ff00;
}

nav{
display:flex;
justify-content:center;
background:#001933;
padding:10px;
}

nav button{
margin:5px;
padding:10px 20px;
background:#f7ff00;
border:none;
font-weight:bold;
cursor:pointer;
}

.section{
display:none;
padding:30px;
}

.active{
display:block;
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:20px;
}

.card{
background:#0a1f44;
border:2px solid #f7ff00;
padding:15px;
border-radius:10px;
text-align:center;
}

.card img{
width:100%;
border-radius:10px;
cursor:pointer;
}

.button{
margin-top:10px;
padding:10px;
background:#f7ff00;
border:none;
font-weight:bold;
cursor:pointer;
width:100%;
}

</style>
</head>

<body>

<header>
<h1>eFootball Account Marketplace</h1>
</header>

<nav>
<button onclick="showSection('market')">Market</button>
<button onclick="showSection('buy')">Buy</button>
<button onclick="showSection('exchange')">Exchange</button>
</nav>

<!-- MARKET SECTION -->
<div id="market" class="section active">
<h2>Market Accounts</h2>

<div class="grid">

<div class="card">
<img src="bmuu.jpg"
onclick="contactWhatsApp('son acct 3172 Strength - $12')" />
<p>Strength: 3172</p>
<p>Price: 120ghc</p>
</div>

<div class="card">
<img src="bmuu1.jpg"
onclick="contactWhatsApp('Legend Account 3193 Strength - $25')" />
<p>Strength: 3193</p>
<p>Price: 250ghc</p>
</div>

</div>

</div>

<!-- BUY SECTION -->
<div id="buy" class="section">
<h2>Buy Account</h2>

<button class="button"
onclick="contactWhatsApp('I want to sell an eFootball account')">
Contact on WhatsApp to Buy
</button>

</div>

<!-- EXCHANGE SECTION -->
<div id="exchange" class="section">
<h2>Exchange Account</h2>

<button class="button"
onclick="contactWhatsApp('I want to exchange my eFootball account')">
Contact on WhatsApp to Exchange
</button>

</div>

<style>
footer{
    background:#001933;
    color:white;
    text-align:center;
    padding:20px;
    margin-top:auto;
}
</style>
<footer>
© 2026 eFootball Market
</footer>

<script>

function showSection(id){
document.querySelectorAll('.section').forEach(sec=>{
sec.classList.remove('active');
});
document.getElementById(id).classList.add('active');
}

function contactWhatsApp(messageText){
let number = "233537112343";  // PUT YOUR NUMBER HERE
let message = encodeURIComponent(messageText);
window.open("https://wa.me/" + number + "?text=" + message, "_blank");
}

</script>

</body>
</html>
