<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<title>Примеры. Добавление квадрата на карту.</title>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
<!--
Подключаем API карт 2.x
Параметры:
- load=package.full - полная сборка;
- lang=ru-RU - язык русский.
-->
<script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU"
<html xmlns="http://www.w3.org/1999/xhtml"> 
<head> 
    <title> Добавление квадрата на карту.</title> 
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/> 
 
    <!-- 
        Подключаем API карт 2.x 
        Параметры: 
          - load=package.full - полная сборка; 
 
      - lang=ru-RU - язык русский. 
    --> 
    <script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU" 
            type="text/javascript"></script> 
    <script type="text/javascript"> 
        ymaps.ready(init); 
 
        function init() { 
            var myMap = new ymaps.Map('map', { 
                center: [-22.57, 17.09], 
                zoom: 8 
            }), 
                myRect = new ymaps.Rectangle([      
                    [-22.60, 17.10], 
                    [-22.72, 17.24]
                ]) 

               ;
                myMap.geoObjects.add(myRect) 
                .add(myGeoObject); 
        } 
    </script> 
</head> 
 
<body> 
<h2>Добавление квадрата на карту</h2> 
 
<div id="map" style="width:600px;height:400px"></div> 
</body> 
 
</html>
