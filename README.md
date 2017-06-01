Это семантическая сеть для визуализации структуры текста.
<script type="text/javascript" 
src="https://www.google.com/jsapi"></script>

<script type="text/javascript">
google.load("visualization", "1.1", 
{packages:["wordtree"]});
 google.setOnLoadCallback(drawChart);
 function drawChart() {
 var data = google.visualization.arrayToDataTable(
 [ ['Фразы'],
 ['текст состоит из вводной части с "фразой-приманкой"'],
 ['текст состоит из вводной части с презентацией темы'],
 ['текст состоит из вводной части с анализом темы'],
 ['текст состоит из вводной части с объяснением проблемы'],
 ['текст состоит из вводной части с планом работы'],
 ['текст состоит из основной части с главами в которых есть параграфы поделенные на абзацы'],
 ['текст состоит из выводов с обобщением промежуточных данных'],
 ['текст состоит из выводов с обобщенным выводом'],
 ['текст состоит из выводов с дальнейшими перспективами размышления'],
 //[''],
 ]
 );
 var options = {
maxFontSize: 14,
 wordtree: {
 format: 'implicit',
 word: 'текст'
 }
 };
 var chart = new google.visualization.WordTree
(document.getElementById('wordtree_basic'));
 chart.draw(data, options);
 }
</script>

<div id="wordtree_basic" style="width: 100%; 
height: 500px;"></div>
