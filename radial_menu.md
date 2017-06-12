//HTML:

<div id='piemenu' data-wheelnav
 data-wheelnav-slicepath='DonutSlice'
 data-wheelnav-marker data-wheelnav-markerpath='PieLineMarker'
 data-wheelnav-rotateoff
 data-wheelnav-navangle='165'
 data-wheelnav-titleheight='30'
 data-wheelnav-cssmode 
 data-wheelnav-init>
  <div data-wheelnav-navitemicon='check' onmouseup='alert("Place your logic here.");'></div>
  <div data-wheelnav-navitemimg='http://pmg.softwaretailoring.net/img/pmg_favicon.png' onmouseup='alert("Place your logic here.");'></div>
  <div data-wheelnav-navitemicon='checkbox' onmouseup='alert("Place your logic here.");'></div>
  <div data-wheelnav-navitemicon='checked' onmouseup='alert("Place your logic here.");'></div>
  <div data-wheelnav-navitemicon='star' onmouseup='alert("Place your logic here.");'></div>
  <div data-wheelnav-navitemicon='icons' onmouseup='alert("Place your logic here.");'></div>
</div>

//Javascript:

var piemenu = new wheelnav('piemenu');
piemenu.clockwise = false;
piemenu.sliceInitPathFunction = piemenu.slicePathFunction;
piemenu.initPercent = 0.1;
piemenu.wheelRadius = piemenu.wheelRadius * 0.83;
piemenu.navItemsContinuous = true;
piemenu.sliceAngle = 30;
piemenu.createWheel();
piemenu.setTooltips(['check','image','checkbox','checked','star','icons']);


//CSS:

#piemenu > svg { width: 100%; height: 100%; }
#piemenu { height: 400px; width: 400px; margin:auto; }
@media (max-width: 400px) { #piemenu { height: 300px; width: 300px; } }

[class|=wheelnav-piemenu-slice-basic] { fill: #497F4C; stroke: none; }
[class|=wheelnav-piemenu-slice-selected] { fill: #497F4C; stroke: none; }
[class|=wheelnav-piemenu-slice-hover] { fill: #497F4C;  stroke: none; fill-opacity: 0.77; cursor: pointer; }

[class|=wheelnav-piemenu-title-basic] { fill: #333; stroke: none; }
[class|=wheelnav-piemenu-title-selected] { fill: #fff; stroke: none; }
[class|=wheelnav-piemenu-title-hover] { fill: #222; stroke: none; cursor: pointer; }

.wheelnav-piemenu-marker { stroke: #444; stroke-width: 2; }