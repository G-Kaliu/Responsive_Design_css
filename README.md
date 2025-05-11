# Responsive_Design_css
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Webpage</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }

    header, footer {
      background: #333;
      color: #fff;
      padding: 1rem;
      text-align: center;
    }

    nav {
      background: #444;
      color: #fff;
      display: flex;
      justify-content: center;
      gap: 1rem;
      padding: 1rem;
      flex-wrap: wrap;
    }

    nav a {
      color: white;
      text-decoration: none;
    }

    .container {
      display: grid;
      grid-template-columns: 1fr 3fr;
      gap: 20px;
      padding: 1rem;
    }

    aside {
      background: #f4f4f4;
      padding: 1rem;
    }

    main {
      background: #e2e2e2;
      padding: 1rem;
    }

    footer {
      margin-top: 2rem;
    }

    @media (max-width: 768px) {
      .container {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 500px) {
      nav {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>My Responsive Webpage</h1>
  </header>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Services</a>
    <a href="#">Contact</a>
  </nav>
  <div class="container">
    <aside>
      <h2>Sidebar</h2>
      <p>This is the sidebar content.</p>
    </aside>
    <main>
      <h2>Main Content</h2>
      <p>This is the main content area. Resize the browser to see the responsive layout in action.</p>
    </main>
  </div>
  <footer>
    <p>&copy; 2025 My Responsive Webpage</p>
  </footer>
</body>
</html>
