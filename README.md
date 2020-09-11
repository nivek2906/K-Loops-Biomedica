# K-Loops-Biomedica
Semana 8 
function setup() {
  createCanvas(800, 800);

}

function draw() {
  background(0);

  var countX = 0;
  var countY = 0;
  var count = 0;

  for (var x = 30; x <= mouseX; x += 50) {
    countX++;
    for (var y = 50; y <= mouseY; y += 50) {
      fill(random(0, 255), random(0, 255), random(0, 255));
      ellipse(x, y, 30);
      count++;
      countY = count / countX;
    }
  }

  fill(0);
  textSize(20);
  text(countX + " X " + countY + " = " + count, 10, 20);

}
