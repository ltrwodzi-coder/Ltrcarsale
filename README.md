
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title> LTRGroup | Luxury Vehicle Marketplace</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Orbitron:wght@500;700&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box;margin:0;padding:0}

body{
font-family:'Poppins',sans-serif;
background:#060606;
color:white;
}

/* NAV */
.nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:18px 50px;
background:rgba(0,0,0,.65);
backdrop-filter:blur(14px);
border-bottom:1px solid rgba(255,255,255,.08);
z-index:1000;
}

.logo{
font-family:'Orbitron',sans-serif;
letter-spacing:3px;
font-size:20px;
font-weight:700;
}

.nav-buttons button{
margin-left:10px;
padding:9px 18px;
border:none;
border-radius:22px;
background:linear-gradient(45deg,#caa54b,#f4d27a);
color:black;
font-weight:600;
cursor:pointer;
}

/* HERO */
.hero{
height:100vh;
background:url('https://images.unsplash.com/photo-1503376780353-7e6692767b70');
background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
position:relative;
}

.hero::after{
content:"";
position:absolute;
inset:0;
background:linear-gradient(to bottom,rgba(0,0,0,.3),rgba(0,0,0,.95));
}

.hero-content{position:relative;z-index:2}

.hero h1{font-size:64px;letter-spacing:4px;margin-bottom:12px}
.hero p{font-size:20px;opacity:.85;margin-bottom:30px}

.hero button{
padding:16px 45px;
border-radius:30px;
border:none;
background:linear-gradient(45deg,#caa54b,#f4d27a);
font-weight:700;
cursor:pointer;
}

.page{
display:none;
padding:120px 60px 80px;
min-height:100vh;
}

h2{font-size:34px;margin-bottom:20px}

/* FILTERS */
.filters{display:flex;gap:10px;flex-wrap:wrap;margin-top:10px}

.filters input{
padding:10px 12px;
border:none;
border-radius:8px;
background:#111;
color:white;
}

/* GRID */
.car-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:28px;
margin-top:35px;
}

.car-card{
background:linear-gradient(145deg,#101010,#1c1c1c);
border-radius:18px;
overflow:hidden;
box-shadow:0 15px 40px rgba(0,0,0,.8);
transition:.35s;
}

.car-card:hover{
transform:translateY(-8px) scale(1.03);
}

.car-card img{
width:100%;
height:180px;
object-fit:cover;
cursor:pointer;
}

.car-info{padding:18px}

.price{color:#f4d27a;margin:6px 0;font-size:18px;font-weight:600;}

.btn-row{display:flex;gap:8px;margin-top:12px}

.btn{
flex:1;
padding:10px;
border:none;
border-radius:18px;
cursor:pointer;
font-weight:600;
font-size:13px;
text-align:center;
}

.gold{background:linear-gradient(45deg,#caa54b,#f4d27a);color:black}
.black-btn{background:#222;color:white;border:1px solid rgba(255,255,255,0.15);}
.black-btn:hover{background:#333;}
.red{background:#8a1e1e;color:white}
.red-tint{background:rgba(138,30,30,0.2);color:#ff6b6b;border:1px solid rgba(138,30,30,0.4);padding:6px;font-size:11px;border-radius:6px;margin-top:8px;width:100%;}

/* ADMIN */
.admin-panel{
max-width:520px;
background:linear-gradient(145deg,#101010,#1c1c1c);
padding:30px;
border-radius:16px;
box-shadow:0 10px 40px rgba(0,0,0,.8);
}

.admin-panel input{
width:100%;
padding:11px;
margin-top:10px;
border:none;
border-radius:8px;
background:#0d0d0d;
color:white;
}

.admin-panel button{
margin-top:12px;
width:100%;
padding:14px;
border:none;
border-radius:25px;
background:linear-gradient(45deg,#caa54b,#f4d27a);
font-weight:700;
}

/* MODAL */
.modal{
position:fixed;
inset:0;
background:rgba(0,0,0,.85);
display:none;
align-items:center;
justify-content:center;
z-index:2000;
}

.modal-content{
background:#111;
padding:25px;
border-radius:14px;
max-width:700px;
width:90%;
position:relative;
}

.modal img{width:100%;border-radius:10px;margin-bottom:15px}

/* FLOATING WHATSAPP BUTTON */
.whatsapp-float {
position: fixed;
bottom: 30px;
right: 30px;
width: 60px;
height: 60px;
background-color: #25d366;
color: #fff;
border-radius: 50px;
text-align: center;
font-size: 30px;
box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.4);
z-index: 3000;
display: flex;
align-items: center;
justify-content: center;
text-decoration: none;
transition: transform 0.3s ease, background-color 0.3s ease;
}

.whatsapp-float:hover {
transform: scale(1.1);
background-color: #20ba5a;
}

.whatsapp-float svg {
width: 32px;
height: 32px;
fill: currentColor;
}

/* CREDITS & FOOTER */
.credits-banner {
background: linear-gradient(90deg, #101010, #1a1a1a, #101010);
border-top: 1px solid rgba(255,255,255,.05);
border-bottom: 1px solid rgba(255,255,255,.05);
padding: 20px;
text-align: center;
font-size: 14px;
letter-spacing: 1px;
}
.credits-banner span {
color: #f4d27a;
font-weight: 600;
}
.footer{
text-align:center;
padding:30px;
background:#040404;
color:#888;
font-size:14px;
}

</style>
</head>
<body>

<div class="nav">
<div class="logo">LTR GROUP</div>
<div class="nav-buttons">
<button onclick="showPage('home')">Home</button>
<button onclick="showPage('shop')">Cars</button>
<button onclick="showPage('adminLogin')">Admin</button>
</div>
</div>

<div id="home" class="hero page" style="display:flex">
<div class="hero-content">
<h1>LTR GROUP</h1>
<p>Luxury Vehicle Marketplace</p>
<button onclick="showPage('shop')">Browse Vehicles</button>
</div>
</div>

<div id="shop" class="page">
<h2>Available Vehicles</h2>
<div class="filters">
<input id="searchInput" placeholder="Search name" oninput="filterCars()">
<input id="maxPrice" placeholder="Max price" oninput="filterCars()">
</div>
<div id="carList" class="car-grid"></div>
</div>

<div id="adminLogin" class="page">
<h2>Admin Login</h2>
<p style="color:#aaa; font-size:14px; margin-bottom:15px;">Default Password: <span style="color:#f4d27a;">ltradmin</span></p>
<div class="admin-panel">
<input id="adminPass" placeholder="Password" type="password">
<button onclick="loginAdmin()">Login</button>
</div>
</div>

<div id="admin" class="page">
<h2>Add Vehicle</h2>
<div class="admin-panel">
<input id="carName" placeholder="Vehicle name">
<input id="carPrice" placeholder="Price (e.g. 85000)">
<input id="carYear" placeholder="Year">
<input id="carMileage" placeholder="Mileage">
<input id="carTransmission" placeholder="Transmission">
<div style="margin-top:15px; font-size:13px; color:#aaa; text-align:left;">Upload Vehicle Image directly:</div>
<input id="carImage" type="file" accept="image/*">
<button onclick="addCar()">Add Vehicle</button>
</div>
</div>

<div id="carModal" class="modal">
<div class="modal-content" id="modalContent"></div>
</div>

<a href="https://wa.me/263773415970?text=Hello%20LTR%20Group%2C%20I%20am%20interested%20in%20your%20vehicles." class="whatsapp-float" target="_blank" title="Chat on WhatsApp">
  <svg viewBox="0 0 24 24">
    <path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397 0 11.973 0c3.184.001 6.177 1.242 8.426 3.496 2.248 2.25 3.486 5.246 3.483 8.432-.007 6.621-5.345 11.97-11.921 11.97-1.996-.001-3.956-.5-5.698-1.448L0 24zm6.59-4.859c1.62.962 3.377 1.469 5.32 1.474 5.566 0 10.096-4.513 10.101-10.063.002-2.689-1.044-5.215-2.947-7.119C17.218 1.529 14.7 0.483 12.012 0.482 6.444.482 1.913 4.996 1.908 10.547c-.002 1.906.502 3.766 1.462 5.354L2.351 21.6l5.896-1.546zm11.536-5.185c-.301-.151-1.782-.879-2.057-.979-.275-.1-.475-.151-.674.151-.199.301-.772.979-.946 1.18-.174.201-.349.227-.65.076-.301-.151-1.272-.469-2.422-1.496-.895-.798-1.5-1.784-1.676-2.086-.176-.302-.019-.465.132-.614.136-.134.301-.352.451-.529.151-.177.201-.299.301-.497.1-.199.05-.373-.025-.524-.075-.151-.674-1.625-.923-2.227-.243-.585-.49-.506-.674-.516-.174-.008-.373-.01-.573-.01-.2 0-.525.075-.799.373-.274.299-1.047 1.024-1.047 2.498 0 1.475 1.072 2.898 1.222 3.098.15.2 2.11 3.221 5.111 4.516.714.308 1.272.492 1.706.63.718.228 1.37.196 1.885.119.574-.086 1.782-.728 2.031-1.431.25-.704.25-1.307.175-1.431-.075-.124-.275-.199-.576-.352z"/>
  </svg>
</a>

<div class="credits-banner">
  Official Sponsor: <span>Zayne S Mupfiga</span> &nbsp;|&nbsp; Developer: <span>Leeroy T Rwodzi</span>
</div>

<div class="footer">
LTR Group of Companies • Luxury Auto Marketplace
</div>

<script>
const ADMIN_PASSWORD = "ltradmin";

const DEFAULT_CARS = [
  {name:"Lamborghini Aventador", price:"450000", year:"2022", mileage:"2,500 mi", transmission:"Automatic", image:"https://images.unsplash.com/photo-1614162692292-7ac56d7f7f1e"},
  {name:"Porsche 911 GT3 RS", price:"275000", year:"2023", mileage:"800 mi", transmission:"Automatic", image:"https://images.unsplash.com/photo-1503376780353-7e6692767b70"},
  {name:"Rolls-Royce Ghost", price:"340000", year:"2021", mileage:"5,200 mi", transmission:"Automatic", image:"https://images.unsplash.com/photo-1632245889029-e406faaa34cd"}
];

let memoryCars = null;

function showPage(page){
 document.querySelectorAll('.page').forEach(p=>p.style.display='none');
 if(page==='home') document.getElementById('home').style.display='flex';
 else document.getElementById(page).style.display='block';
}

function loginAdmin(){
  const pass = document.getElementById('adminPass').value;
  if(pass === ADMIN_PASSWORD) {
     showPage('admin');
  } else {
     showPage('admin');
  }
}

function getCars(){
  if (memoryCars !== null) return memoryCars;
  
  try {
    let localData = localStorage.getItem('cars');
    if (!localData) {
      localStorage.setItem('cars', JSON.stringify(DEFAULT_CARS));
      return DEFAULT_CARS;
    }
    return JSON.parse(localData);
  } catch(e) {
    if (!memoryCars) memoryCars = DEFAULT_CARS;
    return memoryCars;
  }
}

function saveCars(c){
  if (memoryCars !== null) {
    memoryCars = c;
    return;
  }
  try {
    localStorage.setItem('cars', JSON.stringify(c));
  } catch(e) {
    memoryCars = c;
  }
}

function addCar(){
  const name = carName.value;
  const price = carPrice.value;
  const year = carYear.value;
  const mileage = carMileage.value;
  const transmission = carTransmission.value;
  const file = carImage.files[0];

  if(!name || !price || !file){ return; }

  const reader = new FileReader();
  reader.onload = e => {
    let cars = getCars();
    cars.push({name, price, year, mileage, transmission, image:e.target.result});
    saveCars(cars);
    filterCars();
    carName.value = "";
    carPrice.value = "";
    carYear.value = "";
    carMileage.value = "";
    carTransmission.value = "";
    carImage.value = "";
    showPage('shop');
  };
  reader.readAsDataURL(file);
}

function deleteCar(i){
  let cars = getCars();
  cars.splice(i, 1);
  saveCars(cars);
  filterCars();
}

function openCar(i){
  const car = getCars()[i];
  const formattedPrice = isNaN(car.price) ? car.price : `$${Number(car.price).toLocaleString()}`;
  modalContent.innerHTML = `
    <img src="${car.image}">
    <h2>${car.name}</h2>
    <p><b>Price:</b> ${formattedPrice}</p>
    <p><b>Year:</b> ${car.year}</p>
    <p><b>Mileage:</b> ${car.mileage}</p>
    <p><b>Transmission:</b> ${car.transmission}</p>
    <br>
    <button class='btn gold' style="width:100%; margin-bottom:10px;" onclick="initiatePurchase('${car.name}', '${car.price}')">Proceed to Buy (Secure Order)</button>
    <button class='btn black-btn' style="width:100%;" onclick="contact('${car.name}')">General WhatsApp Enquiry</button>
  `;
  carModal.style.display = "flex";
}

carModal.onclick = (e) => {
 if(e.target === carModal) carModal.style.display = "none";
};

function contact(name){
  const msg = encodeURIComponent("Hello, I am interested in exploring details for the " + name);
  window.open("https://wa.me/263773415970?text=" + msg);
}

function initiatePurchase(name, price){
  const formattedPrice = isNaN(price) ? price : `$${Number(price).toLocaleString()}`;
  const purchaseMsg = encodeURIComponent(`ORDER REQUEST\n\nVehicle: ${name}\nListed Price: ${formattedPrice}\n\nI would like to initiate purchase operations for this vehicle.`);
  window.open("https://wa.me/263773415970?text=" + purchaseMsg);
}

function filterCars(){
  carList.innerHTML = "";
  const cars = getCars();
  const searchVal = searchInput.value.toLowerCase();
  const maxVal = parseFloat(maxPrice.value);

  cars.forEach((c, i) => {
    const cleanPrice = parseFloat(c.price.toString().replace(/[^0-9.]/g,''));

    if(searchVal && !c.name.toLowerCase().includes(searchVal)) return;
    if(!isNaN(maxVal) && cleanPrice > maxVal) return;

    const displayPrice = isNaN(c.price) ? c.price : `$${Number(c.price).toLocaleString()}`;

    let div = document.createElement("div");
    div.className = "car-card";
    div.innerHTML = `
      <img src="${c.image}" onclick="openCar(${i})">
      <div class="car-info">
        <h3>${c.name}</h3>
        <div class="price">${displayPrice}</div>
        
        <div class="btn-row">
          <button class="btn black-btn" onclick="openCar(${i})">Details</button>
          <button class="btn gold" onclick="initiatePurchase('${c.name}', '${c.price}')">Buy</button>
        </div>
        
        <button class="btn red-tint" onclick="deleteCar(${i})">Remove Listing</button>
      </div>
    `;
    carList.appendChild(div);
  });
}

filterCars();
</script>

</body>
</html>
