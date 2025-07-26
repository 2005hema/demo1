<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Attractive One-Page Website</title>
  <style>
    /* Reset and base */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body, html {
      height: 100%;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 20px;
    }
    .container {
      background: rgba(0, 0, 0, 0.5);
      border-radius: 15px;
      padding: 40px;
      max-width: 450px;
      box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
      backdrop-filter: blur(8.5px);
      -webkit-backdrop-filter: blur(8.5px);
      border: 1px solid rgba(255, 255, 255, 0.18);
      animation: fadeIn 1.2s ease forwards;
    }
    h1 {
      font-size: 2.8rem;
      margin-bottom: 15px;
      letter-spacing: 2px;
      animation: slideDown 1s ease forwards;
    }
    p {
      font-size: 1.2rem;
      margin-bottom: 30px;
      line-height: 1.5;
      animation: slideUp 1s ease forwards;
    }
    button {
      background-color: #ff6b6b;
      border: none;
      color: white;
      padding: 15px 30px;
      font-size: 1.1rem;
      border-radius: 50px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      box-shadow: 0 4px 15px rgba(255, 107, 107, 0.5);
      animation: pulse 2s infinite;
    }
    button:hover {
      background-color: #ff4757;
      box-shadow: 0 6px 20px rgba(255, 71, 87, 0.7);
    }
    /* Animations */
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
    @keyframes slideDown {
      from {opacity: 0; transform: translateY(-20px);}
      to {opacity: 1; transform: translateY(0);}
    }
    @keyframes slideUp {
      from {opacity: 0; transform: translateY(20px);}
      to {opacity: 1; transform: translateY(0);}
    }
    @keyframes pulse {
      0%, 100% {
        box-shadow: 0 4px 15px rgba(255, 107, 107, 0.5);
      }
      50% {
        box-shadow: 0 8px 30px rgba(255, 107, 107, 0.8);
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Welcome to My Site</h1>
    <p>Experience smooth animations and interactive design, all in one page.</p>
    <button id="magicBtn">Click Me!</button>
  </div>

  <script>
    const button = document.getElementById('magicBtn');

    button.addEventListener('click', () => {
      button.textContent = '✨ You clicked me! ✨';
      button.style.backgroundColor = '#1dd1a1';
      button.style.boxShadow = '0 6px 25px rgba(29, 209, 161, 0.8)';
      setTimeout(() => {
        button.textContent = 'Click Me!';
        button.style.backgroundColor = '#ff6b6b';
        button.style.boxShadow = '0 4px 15px rgba(255, 107, 107, 0.5)';
      }, 3000);
    });
  </script>
</body>
</html>
