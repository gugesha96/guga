<!--preroll - start-->
 <style>#VideOreKLam {position:relative;height:0;z-index:99999;width:100%;float:left;clear:both; margin-left:0px; margin-bottom:0px}</style>
<div id="VideOreKLam">
<div align="right" style="display:none;position: absolute;top: 10px;right: 0px;padding: 5px 10px;background: #000000; font-size: 19px;border-radius: 10px 0 0 10px;z-index:10" id="rek_gec"> <a href="#" onClick="event.preventDefault();/*rekagain();*/document.getElementById('VideOreKLam').parentElement.removeChild(document.getElementById('VideOreKLam'));document.getElementById('player').style.display = 'block';" style="color:#fff"> რეკლამის გათიშვა</a></div>
<div align="right" id="rek_gecmekicin" style="display:none;position: absolute;top: 10px;right: 0px;padding: 5px 10px;background: #000000;border-radius: 10px 0 0 10px;color:#fff;  font-size: 19px; z-index:10">თამაში დაიწყება  <span id="countdown"></span>  წამში</div>
<div  style="position:absolute;display:none;top:0;bottom:0;right:0;left:0;width:100%;height:420px;z-index:9;cursor:pointer" id="viDrekGoster"></div>
<video playsinline autobuffer webkit-playsinline style="object-fit: fill; background:#171717 url('https://sloter.ge/templates/sloter/images/18.png') center no-repeat;background-size:100px;" width="100%" height="633" id="animoGif" poster="https://sloter.ge/templates/sloter/images/18.png">
<source src="https://sloter.ge/promotion/sloter%20promo.mp4" id="myvideo" width="100%" height="633px" onClick="event.preventDefault();window.open('https://guga.ge', '_blank');/*rekagain();*/document.getElementById('VideOreKLam').parentElement.removeChild(document.getElementById('VideOreKLam'));document.getElementById('player').style.display = 'block';">
<source src="http://www.w3schools.com/html/mov_bbb.mp4" id="myvideo" width="100%" height="633px" onClick="event.preventDefault();window.open('https://sloter.ge', '_blank');/*rekagain();*/document.getElementById('VideOreKLam').parentElement.removeChild(document.getElementById('VideOreKLam'));document.getElementById('player').style.display = 'block';">

    </video>
    <video preload="metadata" controls src="https://s3.eu-central-1.amazonaws.com/pipe.public.content/short2.webm" preload="metadata"> </video>

</div>
<script>
var video=document.getElementById('animoGif'); var viDrekGoster=document.getElementById('viDrekGoster');if(viDrekGoster!=null){viDrekGoster.style.display="none"}
video.addEventListener('click',function(){video.play()});video.onplay=function(){if(viDrekGoster!=null){viDrekGoster.style.display="block"}}
video.volume=0.05;
var seconds=5;
function countdown(){seconds=seconds-1;if(seconds<1){document.getElementById('rek_gec').style.display='inline-block';document.getElementById('rek_gecmekicin').style.display='none'}else{document.getElementById("countdown").innerHTML=seconds;window.setTimeout("countdown()",1000)
}}
var vid=document.getElementById("animoGif");vid.onplay=function(){countdown(); 
vid.removeAttribute('controls');vid.style.pointerEvents='none';document.getElementById('viDrekGoster').style.display='block';document.getElementById('rek_gecmekicin').style.display='inline-block'};vid.onended=function(){
if(document.getElementById('VideOreKLam').innerHTML.length>0){document.getElementById('VideOreKLam').parentElement.removeChild(document.getElementById('VideOreKLam'));document.getElementById('player').style.display='block'}};


var vidElement = document.getElementById('myvideo');
var vidSources = [
  "https://sloter.ge/promotion/sloter%20promo.mp4", 
  "http://www.w3schools.com/html/movie.mp4"
  ];
var activeVideo = Math.floor((Math.random() * vidSources.length));
vidElement.src = vidSources[activeVideo];
vidElement.addEventListener('ended', function(e) {
  // update the active video index
  activeVideo = (++activeVideo) % vidSources.length;
  if(activeVideo === vidSources.length){
    activeVideo = 0;
  }

  // update the video source and play
  vidElement.src = vidSources[activeVideo];
  vidElement.play();
});

</script>  
                    <!--preroll - end-->
    
