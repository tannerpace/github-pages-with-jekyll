DJI_0088-HRDDJI_0050-HDR.JPGYou have found the home of Tanner Bleakley

<hr>
I'm glad you are here.  
<hr>
This home is under construction.

<hr>
I would like to share my perspective. I prefer certain hardware. Let me tell you why I fly a Phantom 4 Pro, instead of a Mavic 2 pro.  You may find other pilots who use a Mavic 2 Pro. It is a newer drone. It has a 10-bit color profile and high portability. It is also smaller.  You see DJI is just like the railroad I work for. Their purpose is to make more money at less cost.  You see the Mavic weighs less than the Phantom 4 Pro.  What this means the parts can all be smaller. Batteries are smaller, motors are smaller, even the camera sensor is smaller. The Phantom 4 Pro is bigger. It is more stable. It can shoot 60 fps at 4k. The Mavic2 can only shoot 30 fps at 4k. The Phantom 4 Pro also has a mechanical shutter that is better for mapping. The digital shutter of the Mavic 2 Pro can cause the dreaded rolling shutter effect. Mechanical Shutter


<html><hr>
<body>

<button type="button2" onclick="myFunction3()">Dont waste time clicking here
!</button>
<hr>

<h4>Welcome to My website!</h4>

<p>If You would like to learn more, You can only choose one, neither is a good idea! </p>

<button type="button" onclick="myFunction()">DO NOT CLICK this top button
!</button>

<p id="demo1"></p>
<p id="demo2"></p>

<script>
function myFunction() {
 document.getElementById("demo1").innerHTML = "Why did you click?";
 document.getElementById("demo2").innerHTML = "I TOLD YOU NOT TO!";
}
</script>
<script>
function myFunction2() {
 document.getElementById("demo1").innerHTML = "Im glad you clicked the bottom button :)";
 document.getElementById("demo2").innerHTML = "I can tell you are good at following instructions ;)";
}
</script>
<button type="button" onclick="myFunction2()">Do not click this bottom button
!</button>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
<style>
body {
 background-color: #FFFFFF;
}

h1 {
 color: white;
 text-align: center;
}

p {
 font-family: verdana;
 font-size: 20px;
}
</style>
</head>
<body>
<hr>
<h1>Hi There</h1>
<p>I finally got inside the computer.</p>

</body>
</html>

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {box-sizing: border-box;}

.img-comp-container {
  position: relative;
  height: 200px; /*should be the same height as the images*/
}

.img-comp-img {
  position: absolute;
  width: auto;
  height: auto;
  overflow:hidden;
}

.img-comp-img img {
  display:block;
  vertical-align:middle;
}

.img-comp-slider {
  position: absolute;
  z-index:9;
  cursor: ew-resize;
  /*set the appearance of the slider:*/
  width: 40px;
  height: 40px;
  background-color: #2196F3;
  opacity: 0.7;
  border-radius: 50%;
}
</style>
<script>
function initComparisons() {
  var x, i;
  /*find all elements with an "overlay" class:*/
  x = document.getElementsByClassName("img-comp-overlay");
  for (i = 0; i < x.length; i++) {
    /*once for each "overlay" element:
    pass the "overlay" element as a parameter when executing the compareImages function:*/
    compareImages(x[i]);
  }
  function compareImages(img) {
    var slider, img, clicked = 0, w, h;
    /*get the width and height of the img element*/
    w = img.offsetWidth;
    h = img.offsetHeight;
    /*set the width of the img element to 50%:*/
    img.style.width = (w / 2) + "px";
    /*create slider:*/
    slider = document.createElement("DIV");
    slider.setAttribute("class", "img-comp-slider");
    /*insert slider*/
    img.parentElement.insertBefore(slider, img);
    /*position the slider in the middle:*/
    slider.style.top = (h / 2) - (slider.offsetHeight / 2) + "px";
    slider.style.left = (w / 2) - (slider.offsetWidth / 2) + "px";
    /*execute a function when the mouse button is pressed:*/
    slider.addEventListener("mousedown", slideReady);
    /*and another function when the mouse button is released:*/
    window.addEventListener("mouseup", slideFinish);
    /*or touched (for touch screens:*/
    slider.addEventListener("touchstart", slideReady);
    /*and released (for touch screens:*/
    window.addEventListener("touchstop", slideFinish);
    function slideReady(e) {
      /*prevent any other actions that may occur when moving over the image:*/
      e.preventDefault();
      /*the slider is now clicked and ready to move:*/
      clicked = 1;
      /*execute a function when the slider is moved:*/
      window.addEventListener("mousemove", slideMove);
      window.addEventListener("touchmove", slideMove);
    }
    function slideFinish() {
      /*the slider is no longer clicked:*/
      clicked = 0;
    }
    function slideMove(e) {
      var pos;
      /*if the slider is no longer clicked, exit this function:*/
      if (clicked == 0) return false;
      /*get the cursor's x position:*/
      pos = getCursorPos(e)
      /*prevent the slider from being positioned outside the image:*/
      if (pos < 0) pos = 0;
      if (pos > w) pos = w;
      /*execute a function that will resize the overlay image according to the cursor:*/
      slide(pos);
    }
    function getCursorPos(e) {
      var a, x = 0;
      e = e || window.event;
      /*get the x positions of the image:*/
      a = img.getBoundingClientRect();
      /*calculate the cursor's x coordinate, relative to the image:*/
      x = e.pageX - a.left;
      /*consider any page scrolling:*/
      x = x - window.pageXOffset;
      return x;
    }
    function slide(x) {
      /*resize the image:*/
      img.style.width = x + "px";
      /*position the slider:*/
      slider.style.left = img.offsetWidth - (slider.offsetWidth / 2) + "px";
    }
  }
}
</script>
</head>
<body>

<h1>Compare Two Images</h1>

<p>Click and slide the blue slider to compare two images:</p>

<div class="img-comp-container">
  <div class="img-comp-img">
    <img src="img_DJI_0088-HRD.jpg" width="300" height="200">
  </div>
  <div class="img-comp-img img-comp-overlay">
    <img src="img_DJI_0050.jpg" width="300" height="200">
  </div>
</div>

<script>
/*Execute a function that will execute an image compare function for each element with the img-comp-overlay class:*/
initComparisons();
</script>

</body>
</html>
