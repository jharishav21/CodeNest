# CodeNest
Learn to Code, Grow Your Skills 
<br>
Author - Rishav Jha
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Welcome to CodeSphere</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <section class="welcome">
    <h1>Welcome to <span>CodeSphere</span></h1>
    <p>Your gateway to mastering programming languages.</p>
    <a href="topics.html" class="btn">Get Started</a>
  </section>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Programming Topics</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <section class="topics">
    <h2>Explore Programming Languages</h2>
    <p>Click on a language to access curated notes and video lectures from trusted sources.</p>

    <ul class="language-list">
      <li><a href="https://www.geeksforgeeks.org/c-programming-language/" target="_blank">C Language</a></li>
      <li><a href="https://www.w3schools.com/cpp/" target="_blank">C++</a></li>
      <li><a href="https://www.learnpython.org/" target="_blank">Python</a></li>
      <li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">JavaScript</a></li>
      <li><a href="https://www.w3schools.com/java/" target="_blank">Java</a></li>
      <li><a href="https://www.php.net/manual/en/intro-whatis.php" target="_blank">PHP</a></li>
    </ul>
  </section>

  <section class="rating">
    <h3>Rate Your Experience</h3>
    <div class="stars">
      ★★★★★
    </div>
    <input type="range" min="1" max="5" value="3" id="rating">
    <button onclick="submitRating()">Submit</button>
    <p id="thanksMsg"></p>
  </section>

  <script src="script.js"></script>
</body>
</html>
body {
  font-family: 'Segoe UI', sans-serif;
  margin: 0;
  background: #f9f9f9;
  color: #333;
}

.welcome {
  height: 100vh;
  background: linear-gradient(to right, #4facfe, #00f2fe);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
}

.welcome h1 span {
  color: #fffa65;
}

.btn {
  margin-top: 20px;
  padding: 12px 25px;
  background: #fff;
  color: #4facfe;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
}

.topics {
  padding: 40px;
  max-width: 800px;
  margin: auto;
}

.language-list {
  list-style: none;
  padding: 0;
}

.language-list li {
  margin: 12px 0;
}

.language-list a {
  text-decoration: none;
  color: #007acc;
  font-size: 18px;
}

.rating {
  margin: 40px auto;
  text-align: center;
}

.stars {
  font-size: 30px;
  color: #ffd700;
}

button {
  margin-top: 10px;
  padding: 8px 15px;
  background: #00c853;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

button:hover {
  background: #00a943;
}
function submitRating() {
  const rating = document.getElementById('rating').value;
  document.getElementById('thanksMsg').textContent = `Thank you for rating us ${rating}/5!`;
}

