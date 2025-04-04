<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>QuickBus - Book Your Bus Tickets</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }
    header {
      background: rgba(0, 0, 0, 0.6);
      color: white;
      padding: 20px;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
    }
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1564866657319-08f84a3c7a06') no-repeat center center/cover;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
    }
    .search-section {
      padding: 60px 20px;
      background: #f4f4f4;
    }
    .search-box {
      max-width: 800px;
      margin: auto;
      background: white;
      padding: 30px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    .search-box input, .search-box select, .search-box button {
      padding: 10px;
      margin: 10px 5px;
      width: calc(100% - 22px);
    }
    .video-section {
      text-align: center;
      padding: 40px;
    }
    .video-section iframe {
      width: 80%;
      max-width: 800px;
      height: 450px;
      border: none;
    }
    .bus-listing {
      padding: 40px 20px;
      background: #fff;
    }
    .bus-item {
      background: #f9f9f9;
      padding: 20px;
      margin: 10px 0;
      box-shadow: 0 1px 5px rgba(0,0,0,0.1);
    }
    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <div class="logo">QuickBus</div>
      <div class="nav-links">
        <a href="#">Home</a>
        <a href="#search">Search</a>
        <a href="#video">How It Works</a>
        <a href="#buses">Available Buses</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
  </header>

  <section class="hero">
    <div>
      <h1>Book Your Bus Tickets Online</h1>
      <p>Quick, easy, and affordable!</p>
      <button onclick="document.getElementById('search').scrollIntoView({behavior: 'smooth'})">Search Buses</button>
    </div>
  </section>

  <section class="search-section" id="search">
    <div class="search-box">
      <h2>Search Your Trip</h2>
      <input type="text" placeholder="From">
      <input type="text" placeholder="To">
      <input type="date">
      <select>
        <option value="">Sort By</option>
        <option value="price">Price</option>
        <option value="time">Departure Time</option>
        <option value="duration">Duration</option>
      </select>
      <button>Search</button>
    </div>
  </section>

  <section class="video-section" id="video">
    <h2>How to Book a Bus</h2>
    <iframe src="https://www.youtube.com/embed/l1EssrLxt7E" allowfullscreen></iframe>
  </section>

  <section class="bus-listing" id="buses">
    <h2>Available Buses</h2>
    <div class="bus-item">
      <h3>Express Line - 8:00 AM</h3>
      <p>From City A to City B | Duration: 5h | Price: $20</p>
      <button>Book Now</button>
    </div>
    <div class="bus-item">
      <h3>Comfort Travels - 10:30 AM</h3>
      <p>From City A to City B | Duration: 6h | Price: $25</p>
      <button>Book Now</button>
    </div>
    <div class="bus-item">
      <h3>Night Rider - 9:00 PM</h3>
      <p>From City A to City B | Duration: 5h 30min | Price: $22</p>
      <button>Book Now</button>
    </div>
  </section>

  <footer id="contact">
    <p>&copy; 2025 QuickBus. All rights reserved.</p>
    <p>Contact: support@quickbus.com | Phone: +123 456 7890</p>
  </footer>
</body>
</html>
