<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Paintings & Sketches</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f9f9f9;
      color: #333;
    }
    header {
      text-align: center;
      padding: 50px;
      background: #222;
      color: white;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .gallery img {
      width: 100%;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.2);
    }
    .form-section {
      background: white;
      padding: 30px;
      margin: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.2);
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    input, textarea, button {
      padding: 10px;
      font-size: 16px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      background: #222;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background: #444;
    }
  </style>
</head>
<body>

  <header>
    <h1>My Paintings & Sketches</h1>
    <p>Welcome! Have a look at my artwork and request your own custom piece below.</p>
  </header>

  <!-- Gallery Section -->
  <section class="gallery">
    <img src="painting1.jpg" alt="Painting 1">
    <img src="painting2.jpg" alt="Painting 2">
    <img src="sketch1.jpg" alt="Sketch 1">
    <img src="sketch2.jpg" alt="Sketch 2">
  </section>

  <!-- Form Section -->
  <section class="form-section">
    <h2>Request a Custom Sketch/Painting</h2>
    <form action="https://formspree.io/f/your-form-id" method="POST">
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="email" name="email" placeholder="Your Email" required>
      <input type="text" name="contact" placeholder="Phone/WhatsApp">
      <input type="date" name="date" required>
      <textarea name="details" placeholder="Describe what you want" rows="4"></textarea>
      <button type="submit">Submit Request</button>
    </form>
  </section>

</body>
</html>
