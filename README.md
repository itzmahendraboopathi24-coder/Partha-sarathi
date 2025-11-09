<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Boopathi Electrical Services - Service Booking</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      margin: 0;
      background-color: #f4f6f9;
    }
    header {
      background-color: #004aad;
      color: white;
      text-align: center;
      padding: 20px;
    }
    h1 { margin: 0; }
    .container {
      max-width: 1100px;
      margin: auto;
      padding: 20px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 3px 8px rgba(0,0,0,0.1);
      text-align: center;
      padding: 15px;
      transition: 0.3s;
    }
    .card:hover {
      transform: scale(1.03);
    }
    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 10px;
    }
    h3 {
      color: #004aad;
      margin-top: 10px;
    }
    form {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 3px 8px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin-top: 10px;
      font-weight: 600;
    }
    input, select, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 15px;
    }
    button {
      margin-top: 15px;
      background-color: #004aad;
      color: white;
      border: none;
      padding: 12px 20px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover { background-color: #00337a; }
    footer {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 10px;
      margin-top: 20px;
    }
  </style>
</head>
<body>

<header>
  <h1>Boopathi Electrical Services</h1>
  <p>Expert Appliance Repairs • Palani • 15+ Years Experience</p>
</header>

<div class="container">
  <h2>⚙️ Our Repair Services</h2>
  <div class="grid">
    <div class="card">
      <img src="https://i.imgur.com/7D9xTPa.jpg" alt="Washing Machine" />
      <h3>Washing Machine</h3>
      <p>Brands: LG, Samsung, Whirlpool, IFB, Bosch</p>
      <p>Fully Automatic & Semi Automatic</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/qpPWgBG.jpg" alt="Water Heater" />
      <h3>Water Heater (Geyser)</h3>
      <p>Brands: V-Guard, Racold, Bajaj, AO Smith</p>
      <p>Capacities: 5L - 25L</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/UVmMjrY.jpg" alt="Ceiling Fan" />
      <h3>Ceiling / Table / Pedestal Fan</h3>
      <p>Brands: Usha, Crompton, Havells, Orient</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/cBltC0x.jpg" alt="Grinder" />
      <h3>Table Top & Bed Grinder</h3>
      <p>Brands: Butterfly, Elgi Ultra, Preethi</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/8oM4T2O.jpg" alt="Water Pump" />
      <h3>Water Pump Motor</h3>
      <p>Brands: Texmo, Kirloskar, Sharp</p>
      <p>0.5HP - 2HP</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/7DpScCG.jpg" alt="Induction Stove" />
      <h3>Induction Stove</h3>
      <p>Brands: Pigeon, Prestige, Butterfly</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/NvK6fwG.jpg" alt="Tower Fan" />
      <h3>Tower Fan</h3>
      <p>Brands: Usha, V-Guard, Havells</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/vKHVQKe.jpg" alt="Air Cooler" />
      <h3>Air Cooler</h3>
      <p>Brands: Symphony, Bajaj, Orient, Crompton</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/2TRbKxi.jpg" alt="Stabilizer" />
      <h3>Stabilizer</h3>
      <p>Brands: V-Guard, Everest, Microtek</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/HWz6xiy.jpg" alt="UPS Inverter" />
      <h3>UPS & Inverter</h3>
      <p>Brands: Luminous, Microtek, Exide</p>
    </div>

    <div class="card">
      <img src="https://i.imgur.com/jQbXW6I.jpg" alt="Water Purifier" />
      <h3>Water Purifier</h3>
      <p>Brands: Kent, Aquaguard, Pureit</p>
    </div>
  </div>

  <h2 style="margin-top:40px;">📞 Book a Service Call</h2>
  <form onsubmit="sendWhatsApp(); return false;">
    <label>Customer Name:</label>
    <input type="text" id="name" placeholder="Enter your name" required />

    <label>Contact Number:</label>
    <input type="tel" id="phone" placeholder="Enter your mobile number" required />

    <label>Location / Address:</label>
    <input type="text" id="location" placeholder="Your address or area" required />

    <label>Appliance Type:</label>
    <select id="appliance" required>
      <option value="">--Select Appliance--</option>
      <option>Washing Machine</option>
      <option>Water Heater</option>
      <option>Ceiling Fan</option>
      <option>Table Fan</option>
      <option>Pedestal Fan</option>
      <option>Grinder</option>
      <option>Water Pump</option>
      <option>Water Purifier</option>
      <option>Induction Stove</option>
      <option>Air Cooler</option>
      <option>Stabilizer</option>
      <option>UPS / Inverter</option>
    </select>

    <label>Appliance Brand & Model:</label>
    <input type="text" id="brand" placeholder="e.g., LG T70SJMB1Z" required />

    <label>Problem Description:</label>
    <textarea id="problem" rows="3" placeholder="Describe issue (e.g., not heating, motor jam...)" required></textarea>

    <button type="submit">📩 Book Now on WhatsApp</button>
  </form>
</div>

<footer>
  © 2025 Boopathi Electrical Services | Palani | 9080811393
</footer>

<script>
  function sendWhatsApp() {
    let name = document.getElementById("name").value;
    let phone = document.getElementById("phone").value;
    let location = document.getElementById("location").value;
    let appliance = document.getElementById("appliance").value;
    let brand = document.getElementById("brand").value;
    let problem = document.getElementById("problem").value;

    let msg = `🔧 *New Service Request* 🔧\n\n👤 Name: ${name}\n📞 Contact: ${phone}\n📍 Location: ${location}\n🛠️ Appliance: ${appliance}\n🏷️ Brand/Model: ${brand}\n⚙️ Problem: ${problem}`;
    
    let url = "https://wa.me/919080811393?text=" + encodeURIComponent(msg);
    window.open(url, "_blank");
  }
</script>

</body>
</html>
