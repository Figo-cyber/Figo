<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
    }
.card {
      background: #fff;
      width: 90%;
      max-width: 400px;
      padding: 24px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }
img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #764ba2;
      margin-bottom: 16px;
    }
h3 {
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
      color: white;
      text-decoration: none;
      border-radius: 30px;
    }
.btn:hover {
      background: #667eea;
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
    </p>
    <a href="#" class="btn">Kenalan Yuk</a>
  </div>
</body>
</html>
