<!DOCTYPE html>
<html lang="te">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>మీరు ఒంటరిగా లేరు – మీ ప్రార్థనను పంచుకోండి</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-image: url("https://res.cloudinary.com/dyndhbhkp/image/upload/v1749050842/aufuev0ounfhy4usyj3h.png");
      background-size: cover;
      height: 100vh;
      width: 100vw;
      padding: 20px;
      text-align: center;
      
    }
  
    .form-container {
      background: #fff;
      max-width: 500px;
      margin: auto;
      padding: 30px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 12px;
    }
    h2 {
      color: #2c3e50;
    }
    label {
      display: block;
      margin: 15px 0 5px;
      text-align: left;
      font-weight: bold;
    }
    input, textarea, select {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 16px;
    }
    button {
      margin-top: 20px;
      background-color: #3498db;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }
    .thank-you {
      display: none;
      font-size: 18px;
      color: green;
      margin-top: 20px;
    }
    .logo,
    .logo-image {
      text-align: center;
      margin-bottom: 15px;
    }
    .logo img {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      background-color: #f8f9fa;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      padding: 10px;
    }
    .logo-image img {
      max-width: 750px;
      height: auto;
     border-radius: 30px;
    }
    
  </style>
</head>
<body>
  <div class="logo">
    <img src="https://res.cloudinary.com/dyndhbhkp/image/upload/v1753605453/unnamed_1_hetjy0.png" alt="Prayer Logo">
  </div>
  <div class="logo-image">
    <img src="https://res.cloudinary.com/dyndhbhkp/image/upload/v1753590428/CALVARY_TEMPLE_b3dwfa.png" alt="Calvary Temple Logo">
  </div>
  <div class="form-container">
    <h2>🙏 మీరు ఒంటరిగా లేరు – మీ ప్రార్థనను పంచుకోండి</h2>
    <form id="prayerForm">
      <label for="name">పేరు (Name):</label>
      <input type="text" id="name" name="name" required>

      <label for="phone">ఫోన్ నంబర్ (Phone Number):</label>
      <input type="tel" id="phone" name="phone" required>

      <label for="prayer">మీ ప్రార్థన అభ్యర్థన (Your Prayer Request):</label>
      <textarea id="prayer" name="prayer" rows="5" required></textarea>

      <label for="callback">24 గంటల్లో మీరు కాల్ కావాలనుకుంటున్నారా?</label>
      <select id="callback" name="callback" required>
        <option value="Yes">అవును (Yes)</option>
        <option value="No">కాదు (No)</option>
      </select>

      <label for="visit">మీరు మా చర్చికి రావాలనుకుంటున్నారా?</label>
      <select id="visit" name="visit">
        <option value="Yes">అవును (Yes)</option>
        <option value="No">కాదు (No)</option>
        <option value="Maybe">ఏమో చూద్దాం (Maybe)</option>
      </select>

      <button type="submit">అభ్యర్థన పంపించండి (Submit)</button>
      <div class="thank-you">ధన్యవాదాలు! మేము త్వరలో మిమ్మల్ని సంప్రదిస్తాము మరియు మీ కోసం ప్రార్థిస్తాము.</div>
    </form>
  </div>

  <script>
    document.getElementById('prayerForm').addEventListener('submit', function(e) {
      e.preventDefault();
      document.querySelector('.thank-you').style.display = 'block';
      // TODO: Add integration to backend like Google Sheets or Firebase
    });
  </script>
</body>
</html>
