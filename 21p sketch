int pressed, pressedState;
PImage pilots;
void setup() {
  size(1000, 1000);
  pressed = 0;
  pressedState = 0;
}

void draw() {
  if (pressedState == 0) {
    drawEmblem1();
  } else {
    drawEmblem2();
  }
  if (pressedState == 2) {
    drawImage();
  }
}

void drawEmblem1() {
  noStroke();
  background(0);
  fill(255);
  ellipse(500, 500, 850, 850);
  fill(50, 230, 250);
  beginShape();
  vertex(260, 190);
  vertex(370, 190);
  vertex(370, 820);
  vertex(260, 820);
  endShape();
  fill(250, 20, 20);
  beginShape();
  vertex(730, 210);
  vertex(840, 270);
  vertex(500, 810);
  vertex(390, 740);
  endShape();
  fill(0);
  beginShape();
  vertex(230, 450);
  vertex(730, 450);
  vertex(730, 570);
  vertex(230, 570);
  endShape();
}

void drawEmblem2() {
  background(0);
  noFill();
  stroke(255);
  strokeWeight(15);
  ellipse(500, 500, 800, 800);
  line(350, 300, 350, 700);
  line(440, 500, 540, 500);
  stroke(220, 40, 40);
  line(700, 310, 575, 600);
}

void drawImage(){
  pilots = loadImage("21p.jpg");
  image(pilots, 0,80, width, 830);
}

void mousePressed() {
  pressed = pressed+1;
  pressedState = (pressed%3);
}
