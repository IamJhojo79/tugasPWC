<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Halaman Beranda</title>
  <style>
    body {
      background-image: url('https://github.com/IamJhojo79/tugasPWC/blob/main/Pemandangan-Laut-Raja-Ampat-Yang-Indah.jpg');
      background-size: cover;
      background-position: center;
      font-family: 'kristen itc', sans-serif;
      margin: 0;
      padding: 0;
      overflow: hidden;
    }

    header {
      text-align: center;
      color: whitesmoke;
      text-shadow: -2px -2px 0 #333333, 2px -2px 0 #333333, -2px 2px 0 #333333, 2px 2px 0 #333333;
    }

    #main-content {
      position: relative;
      overflow: hidden;
      height: 100vh;
    }

    #moving-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-60%, -60%);
      font-size: 30px;
      animation: moveText 1s linear infinite;
    }

    /* Style dasar untuk tombol */
    .my-button {
      display: block;
      padding: 20px 40px;
      font-size: 16px;
      text-align: center;
      text-decoration: none;
      cursor: pointer;
      border: 2px solid #f0f0f0;
      color: #f0f0f0;
      border-radius: 5px;
      transition: background-color 0.10s;
    }

    /* Hover effect */
    .my-button:hover {
      background-color: #3498db;
      color: #fff;
    }

    @keyframes moveText {
      0% {
        transform: translate(-50%, -50%);
      }

      25% {
        transform: translate(-50%, -40%);
      }

      50% {
        transform: translate(-50%, -50%);
      }

      75% {
        transform: translate(-50%, -60%);
      }

      100% {
        transform: translate(-50%, -50%);
      }
    }

    #description {
      text-align: center;
      padding: 40px;
      background-color: #ecf0f1;
    }
  </style>
</head>

<body>

  <div id="main-content">
    <div id="moving-text">
      <nav>
        <header>
          <h1>WELCOME TO OUR VACATION</h1>
        </header>
        <a href="presentasiPWC.html" href="#" class="my-button">THIS IS OUR VACATION</a>
      </nav>
    </div>
  </div>

  <script>
    document.addEventListener('mousemove', function (e) {
      const x = e.clientX / window.innerWidth - 0.5;
      const y = e.clientY / window.innerHeight - 0.5;
      document.body.style.transform = 'translate(' + -x * 50 + 'px, ' + -y * 50 + 'px)';
    });
  </script>

</body>

</html>
