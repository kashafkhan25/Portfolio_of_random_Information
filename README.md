<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Random Information Portfolio - README</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(-45deg, #0f172a, #020617, #1e293b, #020617);
      background-size: 400% 400%;
      animation: gradientBG 12s ease infinite;
      color: #e5e7eb;
      line-height: 1.6;
      overflow-x: hidden;
    }

    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .container {
      max-width: 900px;
      margin: auto;
      padding: 40px 20px;
    }

    h1, h2 {
      color: #facc15;
      opacity: 0;
      transform: translateY(20px);
      animation: fadeUp 0.8s ease forwards;
    }

    h1 { animation-delay: 0.2s; }
    h2 { animation-delay: 0.4s; }

    p {
      opacity: 0;
      animation: fadeIn 1s ease forwards;
      animation-delay: 0.6s;
    }

    @keyframes fadeUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeIn {
      to {
        opacity: 1;
      }
    }

    .card {
      background: rgba(30, 41, 59, 0.7);
      backdrop-filter: blur(10px);
      padding: 20px;
      border-radius: 14px;
      margin-bottom: 20px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.4);
      transition: all 0.4s ease;
      transform: translateY(30px);
      opacity: 0;
      animation: fadeUp 0.8s ease forwards;
    }

    .card:nth-child(2) { animation-delay: 0.5s; }
    .card:nth-child(3) { animation-delay: 0.7s; }
    .card:nth-child(4) { animation-delay: 0.9s; }
    .card:nth-child(5) { animation-delay: 1.1s; }

    .card:hover {
      transform: translateY(-8px) scale(1.02);
      box-shadow: 0 12px 40px rgba(0,0,0,0.6);
    }

    code {
      background: #020617;
      padding: 4px 8px;
      border-radius: 6px;
      color: #38bdf8;
    }

    ul {
      padding-left: 20px;
    }

    li {
      margin-bottom: 6px;
      transition: transform 0.2s ease;
    }

    li:hover {
      transform: translateX(6px);
      color: #facc15;
    }

    .badge {
      display: inline-block;
      padding: 6px 12px;
      border-radius: 20px;
      background: #facc15;
      color: #020617;
      font-size: 12px;
      margin-right: 6px;
      transition: all 0.3s ease;
    }

    .badge:hover {
      transform: scale(1.1);
      background: #fde047;
    }

    pre {
      background: #020617;
      padding: 12px;
      border-radius: 8px;
      overflow-x: auto;
    }

    .footer {
      text-align: center;
      margin-top: 40px;
      font-size: 14px;
      color: #94a3b8;
      opacity: 0;
      animation: fadeIn 1s ease forwards;
      animation-delay: 1.5s;
    }

    a {
      color: #38bdf8;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Scroll reveal */
    .hidden {
      opacity: 0;
      transform: translateY(40px);
      transition: all 0.6s ease;
    }

    .show {
      opacity: 1;
      transform: translateY(0);
    }

  </style>
</head>

<body>

<div class="container">

  <h1>📚 Random Information Portfolio</h1>
  <p>
    A modern, interactive portfolio that showcases curated knowledge across multiple domains including
    technology, science, psychology, history, space, and future innovations.
  </p>

  <div class="card hidden">
    <h2>✨ Features</h2>
    <ul>
      <li>📖 Dynamic content rendering</li>
      <li>🎨 Clean UI with Tailwind CSS</li>
      <li>📊 Insightful structured sections</li>
      <li>📌 Interactive Table of Contents</li>
      <li>⬆️ Smooth scrolling experience</li>
      <li>⚙️ Customizable theme system</li>
    </ul>
  </div>

  <div class="card hidden">
    <h2>🛠️ Tech Stack</h2>
    <span class="badge">HTML</span>
    <span class="badge">CSS</span>
    <span class="badge">JavaScript</span>
    <span class="badge">Tailwind</span>
  </div>

  <div class="card hidden">
    <h2>📂 Project Structure</h2>
    <pre>
index.html
README.html
assets/
scripts/
    </pre>
  </div>

  <div class="card hidden">
    <h2>🚀 Getting Started</h2>
    <ol>
      <li>Clone the repository</li>
      <li>Open <code>index.html</code></li>
      <li>Explore the portfolio</li>
    </ol>
  </div>

  <div class="card hidden">
    <h2>📈 Future Improvements</h2>
    <ul>
      <li>Dark/Light mode</li>
      <li>Search functionality</li>
      <li>Backend integration</li>
      <li>User-generated content</li>
    </ul>
  </div>

  <div class="footer">
    <p>© 2025 Random Information Portfolio</p>
    <p>Built for learning & presentation purposes</p>
  </div>

</div>

<script>
  // Scroll Reveal Animation
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add("show");
      }
    });
  });

  document.querySelectorAll(".hidden").forEach(el => observer.observe(el));
</script>

</body>
</html>
