# Salmo_do_Dia
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Salmo do Dia</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f5f5f5;
      text-align: center;
    }
    header {
      padding: 20px;
      background: #2e7d32;
      color: white;
    }
    iframe {
      width: 100%;
      height: 85vh;
      border: none;
    }
  </style>
</head>
<body>

<header>
  <h1>📖 Salmo do Dia</h1>
  <p>Nova Versão Internacional (NVI)</p>
</header>

<iframe id="bibleFrame"></iframe>

<script>
  function getDayOfYear(date) {
    const start = new Date(date.getFullYear(), 0, 0);
    const diff = date - start;
    const oneDay = 1000 * 60 * 60 * 24;
    return Math.floor(diff / oneDay);
  }

  const today = new Date();
  const dayOfYear = getDayOfYear(today);
  const psalmNumber = (dayOfYear % 150) + 1;

  const url = `https://www.bible.com/pt/bible/129/PSA.${psalmNumber}.NVI`;
  document.getElementById("bibleFrame").src = url;
</script>

</body>
</html>
