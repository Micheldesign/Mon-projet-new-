<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Motivation Quotidienne</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background: #fceabb;
      background: linear-gradient(to right, #f8b500, #fceabb);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }
    .quote-box {
      background-color: white;
      padding: 30px;
      border-radius: 15px;
      max-width: 600px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }
    .quote {
      font-size: 1.5em;
      margin-bottom: 20px;
    }
    button {
      background-color: #f8b500;
      border: none;
      padding: 10px 20px;
      font-size: 1em;
      cursor: pointer;
      border-radius: 10px;
    }
    .adsense {
      margin-top: 30px;
      background-color: #eee;
      padding: 10px;
      border-radius: 10px;
      width: 300px;
    }
  </style>
</head>
<body>

  <div class="quote-box">
    <div class="quote" id="quote">"Clique sur le bouton pour ta dose de motivation !"</div>
    <button onclick="generateQuote()">Nouvelle citation</button>
    <div class="adsense">
      <!-- Exemple de pub -->
      <p>[Publicité Google AdSense ici]</p>
    </div>
  </div>

  <script>
    const quotes = [
      "Le succès n'est pas la clé du bonheur. Le bonheur est la clé du succès.",
      "N'attends pas l'opportunité, crée-la.",
      "Ta seule limite, c’est toi-même.",
      "Travaille en silence et laisse ton succès faire du bruit.",
      "La discipline est la clé de ta liberté."
    ];

    function generateQuote() {
      const randomIndex = Math.floor(Math.random() * quotes.length);
      document.getElementById("quote").textContent = `"${quotes[randomIndex]}"`;
    }
  </script>

</body>
</html>