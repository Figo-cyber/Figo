<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Web Perkenalan</title>
  <style>
    * {
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #667eea, #764ba2);
      color: #333;
    }
    .card {
      background: #fff;
      width: 90%;
      max-width: 400px;
      padding: 24px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      animation: fadeIn 1s ease;
    }
    img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 16px;
      border: 4px solid #764ba2;
    }
    h1 {
      margin: 10px 0 5px;
    }
    h3 {
      margin: 0 0 15px;
      color: #666;
      font-weight: normal;
    }
    p {
      font-size: 14px;
      line-height: 1.6;
    }
    .btn {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      background: #764ba2;
      color: #fff;
      text-decoration: none;
      border-radius: 30px;
      transition: 0.3s;
    }
    .btn:hover {
      background: #667eea;
      transform: scale(1.05);
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <div class="card">
    <img src="https://via.placeholder.com/150" alt="Foto Profil">
    <h1>Halo, Aku Figo 👋</h1>
    <h3>Pelajar & Calon Programmer</h3>
    <p>
      Aku suka belajar teknologi, matematika, dan membuat website sederhana.
      Web ini adalah contoh web perkenalan yang simpel, rapi, dan langsung bisa dipakai.
    </p>
    <a class="btn" href="#">Kenalan Yuk</a>
  </div>
</body>
</html>
