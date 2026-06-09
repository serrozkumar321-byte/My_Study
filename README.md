<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Online Teaching Hub</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; background: #f4f4f4; }
    header { background: #2c3e50; color: #fff; padding: 20px; text-align: center; }
    nav { margin-top: 10px; }
    nav a { margin: 0 15px; color: #fff; text-decoration: none; }
    section { padding: 20px; }
    .video-container { display: flex; flex-wrap: wrap; gap: 20px; }
    .video-card { background: #fff; padding: 15px; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); width: 300px; }
    .video-card iframe { width: 100%; height: 180px; border-radius: 5px; }
    .form-section { background: #ecf0f1; padding: 20px; border-radius: 8px; }
    footer { background: #2c3e50; color: #fff; text-align: center; padding: 10px; }
    button { background: #3498db; color: #fff; border: none; padding: 10px 15px; border-radius: 5px; cursor: pointer; }
    button:hover { background: #2980b9; }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to My Teaching Hub</h1>
    <nav>
      <a href="#lectures">Lectures</a>
      <a href="#resources">Resources</a>
      <a href="#feedback">Feedback</a>
    </nav>
  </header>

  <section id="lectures">
    <h2>Video Lectures</h2>
    <div class="video-container">
      <div class="video-card">
        <h3>Lecture 1: Thermodynamics Basics</h3>
        <iframe src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
      </div>
      <div class="video-card">
        <h3>Lecture 2: Boiler Systems</h3>
        <iframe src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
      </div>
    </div>
  </section>

  <section id="resources">
    <h2>Downloadable Resources</h2>
    <p><a href="notes.pdf" download>Download Lecture Notes (PDF)</a></p>
  </section>

  <section id="feedback" class="form-section">
    <h2>Feedback Form</h2>
    <form onsubmit="submitForm(event)">
      <label for="name">Name:</label><br>
      <input type="text" id="name" required><br><br>
      <label for="feedback">Your Feedback:</label><br>
      <textarea id="feedback" rows="4" required></textarea><br><br>
      <button type="submit">Submit</button>
    </form>
    <p id="response"></p>
  </section>

  <footer>
    <p>&copy; 2026 My Teaching Hub</p>
  </footer>

  <script>
    function submitForm(event) {
      event.preventDefault();
      document.getElementById('response').innerText = "Thank you for your feedback!";
    }
  </script>
</body>
</html>
