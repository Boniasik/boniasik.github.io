# boniasik.github.io
< script type="text/javascript" 
src="https://www.google.com/jsapi"></script>
google.load("visualization", "1.1", 
{packages:["wordtree"]});
 google.setOnLoadCallback(drawChart);
 function drawChart() {
 var data = google.visualization.arrayToDataTable(
 [ ['Фразы'],
 ['кот друг собаки'],
 ['кот друг человека'],
 ['кот любит мяукать'],
 ['кот любит спать утром'],
 ['кот любит спать днем'],
 ['кот любит прыгать'],
 ['кот любит есть колбасу'],
 ['кот любит есть конфеты'],
 ['кот любит есть мышей'],
 ['кот любит лазить в окно'],
 ['кот любит лазить в шкаф'],
 ['кот любит лазить на дерево'],
 ['кот любит лазить на забор'],
 ['кот любит пить молоко'],
 ['кот любит пить лимонад'],
 ['кот гуляет днем'],
 ['кот гуляет вечером'],
 ['кот живет с человеком'],
 ['кот живет долго'],
 ['кот гуляет ночью'],
 ['кот гуляет ночью один'],
 ]
 );
 var options = {
maxFontSize: 14,
 wordtree: {
 format: 'implicit',
 word: 'кот'
 }
 };
 var chart = new google.visualization.WordTree
(document.getElementById('wordtree_basic'));
 chart.draw(data, options);
 }
<div id="wordtree_basic" style="width: 100%; 
height: 500px;"></div>
