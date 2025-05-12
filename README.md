# Asya
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Asya Ülkeleri Hakkında Bilgiler</title>
  <style>
    body { font-family: Arial, sans-serif; padding: 20px; background-color: #f4f4f4; }
    h1 { text-align: center; }
    .country-list { display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; }
    .country-button {
      background-color: #4CAF50; color: white; padding: 10px 20px;
      border: none; border-radius: 5px; cursor: pointer;
    }
    .country-info { display: none; margin-top: 20px; padding: 15px; background-color: white; border-radius: 8px; }
  </style>
</head>
<body>
  <h1>Asya Ülkeleri Hakkında Bilgiler</h1>
  <div class="country-list">
    <button class="country-button" onclick="showInfo('cin')">Çin</button>
    <button class="country-button" onclick="showInfo('japonya')">Japonya</button>
    <button class="country-button" onclick="showInfo('hindistan')">Hindistan</button>
  </div>

  <div id="cin" class="country-info">
    <h2>Çin</h2>
    <p><strong>Başkent:</strong> Pekin</p>
    <p><strong>Nüfus:</strong> 1.4 milyar</p>
    <p><strong>Resmî Dil:</strong> Çince (Mandarin)</p>
    <p><strong>Önemli Yerler:</strong> Çin Seddi, Yasak Şehir</p>
  </div>

  <div id="japonya" class="country-info">
    <h2>Japonya</h2>
    <p><strong>Başkent:</strong> Tokyo</p>
    <p><strong>Nüfus:</strong> 125 milyon</p>
    <p><strong>Resmî Dil:</strong> Japonca</p>
    <p><strong>Önemli Yerler:</strong> Fuji Dağı, Kyoto Tapınakları</p>
  </div>

  <div id="hindistan" class="country-info">
    <h2>Hindistan</h2>
    <p><strong>Başkent:</strong> Yeni Delhi</p>
    <p><strong>Nüfus:</strong> 1.4 milyar</p>
    <p><strong>Resmî Diller:</strong> Hintçe, İngilizce</p>
    <p><strong>Önemli Yerler:</strong> Tac Mahal, Kutsal Ganj Nehri</p>
  </div>

  <script>
    function showInfo(id) {
      const infos = document.querySelectorAll('.country-info');
      infos.forEach(info => info.style.display = 'none');
      document.getElementById(id).style.display = 'block';
    }
  </script>
</body>
</html>
