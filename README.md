<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Xem video nóng</title>

  <!-- ✅ Ngăn Facebook hiển thị ảnh preview -->
  <meta property="og:title" content="🔥 Xem chi tiết tại đây">
  <meta property="og:description" content="Nhấn để xem nội dung đầy đủ">
  <meta property="og:url" content="https://YOUR-LINK-HERE">
  <meta property="og:type" content="website">
  <!-- Ảnh trắng 1x1 để không hiện preview -->
  <meta property="og:image" content="https://via.placeholder.com/1x1.png">
  <meta property="og:image:width" content="1">
  <meta property="og:image:height" content="1">
  <!-- Ngăn Twitter, Zalo... lấy ảnh -->
  <meta name="twitter:card" content="summary">
  <meta name="twitter:title" content="🔥 Xem chi tiết tại đây">
  <meta name="twitter:description" content="Nhấn để xem nội dung đầy đủ">
  <meta name="twitter:image" content="https://via.placeholder.com/1x1.png">

  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    #popupOverlay {
      position: fixed;
      inset: 0;
      background-color: rgba(0, 0, 0, 0.85);
      display: none;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      z-index: 9999;
    }
    #popupOverlay img {
      max-width: 90%;
      height: auto;
      border-radius: 10px;
    }
    #popupOverlay button {
      margin-top: 20px;
      padding: 12px 24px;
      font-size: 17px;
      font-weight: bold;
      background-color: #ff4444;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      transition: background-color 0.3s;
    }
    #popupOverlay button:hover {
      background-color: #e60000;
    }
    #baitContent * {
      pointer-events: none;
    }
    #baitContent {
      padding: 20px;
      cursor: pointer;
    }
    #realContent {
      display: none;
      padding: 20px;
    }
  </style>
</head>
<body>

  <!-- ✅ Popup -->
  <div id="popupOverlay">
    <img alt="Popup Image" src="https://iili.io/FKJFHdJ.md.jpg" />
    <button onclick="closePopup()">▶ Xem và quay lại để xem video</button>
  </div>

  <!-- ✅ Vùng mồi -->
  <div id="baitContent" onclick="showPopup()">
    <h2>🔥 Link xem:</h2>
    <a href="#">👉 Bấm vào đây</a>
  </div>

  <!-- ✅ Nội dung thật -->
  <div id="realContent">
    <h2>🎬 Nội dung chính:</h2>
    <a href="https://s.shopee.vn/AKPGSeaY1C" target="_blank" rel="noopener noreferrer">👉 Xem video ở đây</a>
  </div>

  <script>
    function showPopup() {
      document.getElementById("popupOverlay").style.display = "flex";
    }
    function closePopup() {
      // Mở link TikTok trước
      window.open("https://vt.tiktok.com/ZSky76wu3/", "_blank", "noopener,noreferrer");
      // Ẩn popup và mồi, hiện nội dung thật
      document.getElementById("popupOverlay").style.display = "none";
      document.getElementById("baitContent").style.display = "none";
      document.getElementById("realContent").style.display = "block";
    }
  </script>

</body>
</html>
