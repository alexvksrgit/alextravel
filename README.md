<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Solo Travel Connect</title>
  <link rel="stylesheet" href="styles.css" />
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to right, #f0f8ff, #e6ffe6);
      color: #333;
    }
    header {
      background-color: #ff6f61;
      color: white;
      padding: 1rem;
    }
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }
    nav ul {
      list-style-type: none;
      display: flex;
      gap: 1rem;
    }
    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    section {
      padding: 2rem;
    }
    .destinations-grid, .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 1rem;
    }
    .destination, .gallery-grid img {
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .destination img, .gallery-grid img {
      width: 100%;
      height: 150px;
      object-fit: cover;
    }
    form input, form textarea, form button {
      display: block;
      width: 100%;
      margin: 0.5rem 0;
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    form button {
      background-color: #28a745;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    footer {
      text-align: center;
      background-color: #333;
      color: white;
      padding: 1rem;
    }
    #connect {
      background-color: #fff8e1;
      padding: 2rem;
      border-top: 2px solid #ff6f61;
    }
    .connect-cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
    }
    .card {
      background: #ffffff;
      border-radius: 10px;
      padding: 1rem;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .card h4 {
      margin-top: 0;
      color: #ff6f61;
    }
    #memories {
      margin-top: 2rem;
    }
    #memories h3 {
      margin-bottom: 1rem;
    }
    #memories-list {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    .memory {
      border: 1px solid #ddd;
      border-radius: 10px;
      padding: 1rem;
      background-color: #fefefe;
      box-shadow: 0 2px 4px rgba(0,0,0,0.05);
    }
    .memory img {
      max-width: 100%;
      height: auto;
      border-radius: 8px;
      margin-top: 0.5rem;
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <h1>Solo Travel Connect</h1>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#destinations">Destinations</a></li>
        <li><a href="#plans">Low-Cost Plans</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#connect">Connect</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home">
    <h2>Where Solo Journeys Become Shared Stories</h2>
    <p>Connect with fellow travelers, share experiences, and explore the world together through this vibrant platform made just for solo explorers.</p>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>We are a growing community of solo adventurers united by the thrill of discovering new places and forming genuine human connections. Our mission is to make solo travel more social, safe, and fun.</p>
  </section>

  <section id="destinations">
    <h2>Popular Destinations in India</h2>
    <div class="destinations-grid">
      <div class="destination"> <img src="images/manali.jpg" alt="Manali" /><p>Manali</p></div>
      <div class="destination"> <img src="images/shimla.jpg" alt="Shimla" /><p>Shimla</p></div>
      <div class="destination"> <img src="images/haridwar.jpg" alt="Haridwar" /><p>Haridwar</p></div>
      <div class="destination"> <img src="images/tajmahal.jpg" alt="Taj Mahal" /><p>Taj Mahal</p></div>
      <div class="destination"> <img src="images/goa.jpg" alt="Goa" /><p>Goa</p></div>
      <div class="destination"> <img src="images/jaipur.jpg" alt="Jaipur" /><p>Jaipur</p></div>
    </div>
  </section>

  <section id="plans">
    <h2>Travel at Low Cost</h2>
    <ul>
      <li><strong>Backpacking on a Budget:</strong> Use local transport, pack light, and choose multipurpose items. Travel overnight to save on stays and join group tours to cut individual costs.</li>
      <li><strong>Affordable Stays:</strong> Try hostels, homestays, or platforms like Couchsurfing. Booking in advance or during the off-season can save a lot.</li>
      <li><strong>Food Hacks:</strong> Eat at local dhabas, street food vendors, or use kitchen access in hostels. Carry dry snacks and a water bottle to refill.</li>
    </ul>
  </section>

  <section id="gallery">
    <h2>Traveler Memories</h2>
    <div class="gallery-grid">
      <img src="images/memory1.jpg" alt="Memory 1">
      <img src="images/memory2.jpg" alt="Memory 2">
      <img src="images/memory3.jpg" alt="Memory 3">
      <img src="images/memory4.jpg" alt="Memory 4">
      <img src="images/memory5.jpg" alt="Memory 5">
      <img src="images/memory6.jpg" alt="Memory 6">
      <img src="images/memory7.jpg" alt="Memory 7">
      <img src="images/memory8.jpg" alt="Memory 8">
      <img src="images/memory9.jpg" alt="Memory 9">
      <img src="images/memory10.jpg" alt="Memory 10">
    </div>
    <form id="upload-form">
      <h3>Share Your Memory</h3>
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="file" name="image" accept="image/*" required>
      <textarea name="story" placeholder="Write something about this memory..." required></textarea>
      <button type="submit">Upload</button>
    </form>
    <div id="memories">
      <h3>Shared Memories</h3>
      <div id="memories-list"></div>
    </div>
  </section>

  <section id="connect">
    <h2>Connect with Fellow Travelers</h2>
    <div class="connect-cards">
      <div class="card">
        <h4>Find a Travel Buddy</h4>
        <p>Looking for someone to explore the Himalayas or roam the streets of Goa with? Post a buddy request!</p>
      </div>
      <div class="card">
        <h4>Start a Conversation</h4>
        <p>Join the community forum to ask questions, share tips, or plan spontaneous meetups.</p>
      </div>
      <div class="card">
        <h4>Share Your Profile</h4>
        <p>Let others know your interests, upcoming plans, and what kind of travel partner you're looking for.</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="email" name="email" placeholder="Your Email" required>
      <textarea name="message" placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Solo Travel Connect. All rights reserved.</p>
    <p>Follow us on Instagram | Facebook | Twitter</p>
  </footer>

  <script>
    document.getElementById('upload-form').addEventListener('submit', function(e) {
      e.preventDefault();
      const name = this.name.value;
      const story = this.story.value;
      const image = this.image.files[0];

      if (name && story && image) {
        const reader = new FileReader();
        reader.onload = function(event) {
          const memoryHTML = `
            <div class="memory">
              <strong>${name}</strong>
              <p>${story}</p>
              <img src="${event.target.result}" alt="Uploaded Memory">
            </div>
          `;
          document.getElementById('memories-list').innerHTML += memoryHTML;
        };
        reader.readAsDataURL(image);

        this.reset();
      }
    });
  </script>
</body>
</html>
# alextravel
