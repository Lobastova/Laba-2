<html xmlns="http://www.w3.org/1999/xhtml">
 <head>    
 <title>Примеры. Добавление прямоугольника на карту.</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>  
    <!--         Подключаем API карт 2.x
         Параметры:
           - load=package.full - полная сборка;
        - lang=ru-RU - язык русский.     -->
      <script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"
             type="text/javascript"></script>
     <script type="text/javascript"> 
        ymaps.ready(init);  
        function init() { 
            var myMap = new ymaps.Map('map', { 
                center: [-25.30, -57.63], 
                zoom: 11           
 }),            
                 
 myPolygon = new ymaps.Polygon([[
                    // Координаты вершин внешней границы многоугольника.
			[-25.25,-57.65],
			[-25.23,-57.55],
			[-25.30,-57.50],
			[-25.37,-57.55],
			[-25.38,-57.65],
			[-25.31,-57.70]
                ]]);
  
            myMap.geoObjects.add(myPolygon)
                 .add(myPolygon); 
        }     </script> 
</head>  
<body> 
<h2>Добавление прямоугольника на карту</h2>  
<div id="map" style="width:600px;height:400px"></div> </body>  
</html>  
 
