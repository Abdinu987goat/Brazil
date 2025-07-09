<!DOCTYPE html>
<html>
<head>
  <title>Мой браузер</title>
</head>
<body>
  <h1>Поиск в Google</h1>
  <input type="text" id="search" placeholder="Введите запрос">
  <button onclick="search()">Найти</button>

  <script>
    function search() {
      const query = document.getElementById('search').value;
      const url = "https://www.google.com/search?q=" + encodeURIComponent(query);
      window.open(url, "_blank");
    }
  </script>
</body>
</html>
