# SS-DYNAMIC-CARGO
SS DYNAMIC CARGO Logistics Forwarder 🇨🇳China to Malaysia🇲🇾
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SS DYNAMIC CARGO</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(
rgba(0,0,0,0.8),
rgba(0,0,0,0.8)),
url('https://images.unsplash.com/photo-1529070538774-1843cb3265df');
background-size:cover;
background-position:center;
background-attachment:fixed;
color:white;
}

header{
text-align:center;
padding:50px 20px;
background:rgba(255,0,0,0.8);
}

header h1{
font-size:45px;
}

header h2{
font-size:22px;
margin-top:10px;
}

.container{
width:90%;
max-width:1200px;
margin:auto;
padding:20px;
}

.section{
background:rgba(0,0,0,0.75);
padding:25px;
margin:20px 0;
border-radius:15px;
border:2px solid red;
}

.section h2{
color:#ff0000;
margin-bottom:20px;
}

input,
textarea,
button{
width:100%;
padding:12px;
margin:8px 0;
border:none;
border-radius:8px;
}

input,
textarea{
background:#f5f5f5;
}

button{
background:red;
color:white;
font-weight:bold;
cursor:pointer;
}

button:hover{
background:#cc0000;
}

.result{
margin-top:15px;
padding:15px;
background:#111;
border-radius:10px;
}

.flag{
font-size:40px;
}

footer{
text-align:center;
padding:20px;
background:black;
margin-top:30px;
}

.whatsapp{
position:fixed;
right:20px;
bottom:20px;
background:#25D366;
color:white;
padding:15px 20px;
border-radius:50px;
text-decoration:none;
font-weight:bold;
box-shadow:0 0 10px rgba(0,0,0,0.5);
}

</style>
</head>

<body>

<header>

<div class="flag">🇨🇳 ➜ 🇲🇾</div>

<h1>SS DYNAMIC CARGO</h1>

<h2>
Logistics Forwarder China to Malaysia
</h2>

<p>
Air Freight | Sea Freight | Door To Door Delivery
</p>

</header>

<div class="container">

<!-- CBM Calculator -->

<div class="section">

<h2>CBM Calculator</h2>

<input type="number" id="length" placeholder="Length (cm)">

<input type="number" id="width" placeholder="Width (cm)">

<input type="number" id="height" placeholder="Height (cm)">

<input type="number" id="qty" placeholder="Quantity">

<button onclick="calculateCBM()">
Calculate
</button>

<div class="result" id="cbmResult">
Result will appear here
</div>

</div>

<!-- Order Form -->

<div class="section">

<h2>Order Form</h2>

<form>

<input type="text" placeholder="Full Name">

<input type="text" placeholder="WhatsApp Number">

<input type="email" placeholder="Email">

<textarea placeholder="Address"></textarea>

<textarea placeholder="Product Item Name / Product Link"></textarea>

<button type="submit">
Submit Order
</button>

</form>

</div>

<!-- Tracking -->

<div class="section">

<h2>Tracking Number</h2>

<input type="text"
placeholder="China Domestic Tracking Number">

<input type="text"
placeholder="Malaysia Courier Tracking Number">

<button>
Track Shipment
</button>

</div>

<!-- Contact -->

<div class="section">

<h2>Contact Us</h2>

<p>
📦 Guangzhou Warehouse
</p>

<p>
📦 Shenzhen Warehouse
</p>

<p>
📦 Yiwu Warehouse
</p>

<br>

<p>
📱 WhatsApp:
+60 11-5145 3147
</p>

<p>
📧 Email:
ssdynamiccargo@gmail.com
</p>

</div>

</div>

<footer>

<h3>
SS DYNAMIC CARGO
</h3>

<p>
Logistics Forwarder China 🇨🇳 to Malaysia 🇲🇾
</p>

</footer>

<a class="whatsapp"
href="https://wa.me/601151453147"
target="_blank">
WhatsApp
</a>

<script>

function calculateCBM(){

let length =
parseFloat(document.getElementById("length").value);

let width =
parseFloat(document.getElementById("width").value);

let height =
parseFloat(document.getElementById("height").value);

let qty =
parseFloat(document.getElementById("qty").value);

let cbm =
(length * width * height * qty) / 1000000;

let air6000 =
(length * width * height * qty) / 6000;

document.getElementById("cbmResult").innerHTML =
`
<h3>Calculation Result</h3>

<p><b>CBM:</b> ${cbm.toFixed(4)} m³</p>

<p><b>Air Freight (6000):</b>
${air6000.toFixed(2)} KG</p>

`;

}

</script>

</body>
</html>
