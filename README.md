<!DOCTYPE html>
<!-- saved from url=(0033)http://www.duocoo.com/love/0o6o0/ -->
<html><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8"> 
   <style type="text/css">
      .words {
    font-size: 150px;
    font-family: 'Regular', cursive;
    width: auto;
    text-align: center;
}
   .days {
    font-size: 216px;
    font-family: 'Rye', cursive;
    width: auto;
    text-align: center;
}

.days-label {
    font-size: 54px;
}

.seconds {
    margin-top: 32px;
    font-size: 32px;
    font-family: "Monda_bo", Georgia, sans-serif;
    width: auto;
    text-align: center;
}

.seconds-label {
     margin-top: 32px;
    font-size: 32px;
    font-family: "Monda_no", Georgia, sans-serif;
    width: auto;
    text-align: center; 
}

.container {
    position: absolute;
}

@font-face {
  font-family: 'Regular';
  font-style: normal;
  font-weight: 400;
  src: local('Rye Regular'), local('Rye-Regular'), url('./jscss/text1.ttf') format('woff');
}

@font-face {
  font-family: 'Rye';
  font-style: normal;
  font-weight: 400;
  src: local('Rye Regular'), local('Rye-Regular'), url('./jscss/Clockopia.ttf') format('woff');
}
@font-face {
  font-family: 'Monda_no';
  font-style: normal;
  font-weight: normal;
  src: local('Monda'), local('Monda-Regular'), url('./jscss/Monda-Regular.ttf') format('truetype');
}
@font-face {
  font-family: 'Monda_bo';
  font-style: normal;
  font-weight: bold;
  src: local('Monda Bold'), local('Monda-Bold'), url('./jscss/Monda-Bold.ttf') format('truetype');
}

   </style>
    <meta http-equiv="X-UA-Compatible" content="IE=8"> 
    <title>Since The Day</title> 
   
    <script src="./jscss/jquery-1.8.3.min.js" type="text/javascript"></script> 
    <script type="text/javascript">
    $(window).resize(function(){
    console.log(parseInt(($(window).width() - $('.container').outerWidth())/2) + 'px');
    $('.container').css({
        position:'absolute',
        left: ($(window).width() - $('.container').outerWidth())/2,
        top: ($(window).height() - $('.container').outerHeight())/2
    });
    console.log($('.container').css('left'));
});

document.ready = function() {
    $(window).resize();
    updateNumbers();
};


function updateNumbers() {
    //var start_time = 1253980800;
    var beginTime = "2020-3-9 00:00:00";  
    var start_time = Date.parse(beginTime)
   // var start_time =  new Date("2014-11-11 10:10:10").Format("yyyy-MM-dd hh:mm:ss");
    var duration = parseInt(Date.now()- start_time)/1000;

    var seconds = parseInt( duration % 60);
    if (seconds < 10)
        seconds = "0" + seconds;
    duration = parseInt(duration / 60);
    var minutes = duration % 60;
    if (minutes < 10)
        minutes = "0" + minutes;
    duration = parseInt(duration / 60);
    var hours = duration % 24;
    if (hours < 10)
        hours = "0" + hours;
    duration = parseInt(duration / 24);
    var days = duration;
    $('.days-number').text("" + days);
    $('.seconds').text(hours + " hours " + minutes + " minutes " + seconds + " seconds");
    setTimeout("updateNumbers()", 1000);
}
</script> 
    <!--[if lte IE 7]>
    <script type="text/javascript" src="/static/js/degrade.js"></script>
    <![endif]--> 
  </head> 
  <body style="background-color: #e7a3c1"> 
    <div class="container" style="position: absolute; left: 482px; top: 181.5px;">
      <div class="words"> 写程序</div>
      <div class="days">
        <span class="days-number">1921</span>
        <span class="days-label">days</span>
      </div>
      <div class="seconds">15 hours 24 minutes 30 seconds</div>
    </div>   
 <em><em>
</body>
<img src="/images/logo.png" width="258" height="39" />
<time>=“2021/2/7/14:51”
</html>
