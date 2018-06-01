<html>
<head>
  <meta charset="UTF-8">
  <script language="javascript" type="text/javascript" src="https://github.com/processing/p5.js/releases/download/0.5.16/p5.js"></script>
   <script language="javascript" type="text/javascript" src="game.js"></script>
  
  var x = 255;
var y = 100;
PImage img;
void setup() {
  size(600, 440);
  img = loadImage("espaço.jpg");
}

function draw() {
  background(img);;
  if (keyIsDown(LEFT_ARROW))
    x-=5;

  if (keyIsDown(RIGHT_ARROW))
    x+=5;

  if (keyIsDown(UP_ARROW))
    y-=5;

  if (keyIsDown(DOWN_ARROW))
    y+=5;

  ellipse(x, y, 50, 50);
rect(250, 250, 55, 55);
}

  
  <style> body {padding: 0; margin: 0;} </style>
</head>

<body>
</body>
</html> 
