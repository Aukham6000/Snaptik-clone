# Snaptik-clone
simple TikTok video downloader clone
<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SnapTik Downloader</title>
  <style>
    body {
      font-family: sans-serif;
      margin: 0;
      padding: 0;
      background-color: #ffffff;
      text-align: center;
    }
    header {
      background-color: #0063e5;
      padding: 1rem;
      color: white;
    }
    .container {
      padding: 2rem;
    }
    input[type="text"] {
      padding: 10px;
      width: 80%;
      max-width: 500px;
      margin-top: 20px;
    }
    button {
      background-color: #04b35c;
      color: white;
      padding: 10px 20px;
      margin-top: 10px;
      border: none;
      cursor: pointer;
      font-size: 1rem;
    }
    button:hover {
      background-color: #03994d;
    }
  </style>
</head>
<body>
  <header>
    <h1>Download Video TikTok HD</h1>
    <p>No Watermark. เร็ว. อุปกรณ์ทั้งหมด</p>
  </header>
  <div class="container">
    <input type="text" id="tiktokUrl" placeholder="วางลิงก์ TikTok ที่นี่">
    <br>
    <button onclick="downloadVideo()">Download</button>
  </div>

  <script>
    function downloadVideo() {
      const url = document.getElementById('tiktokUrl').value;
      if (!url) {
        alert('กรุณาใส่ลิงก์ TikTok ก่อน');
        return;
      }
      // ปกติจะต้องใช้ backend เพื่อจัดการดาวน์โหลดจริง
      alert(`กำลังพยายามดาวน์โหลดจากลิงก์: ${url}`);
    }
  </script>
</body>
</html>
