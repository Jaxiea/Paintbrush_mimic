float maxWid = 150;
float currentWid = maxWid;
PVector de_po = new PVector(0, 0);
PVector de_acc = new PVector(10, 10);
float rotate_v = 10;
float scale_v = 0.9;

void setup(){
    size(800, 800);
    background(0);
    smooth();
    noStroke();
    frameRate(400);
}

void draw(){
  
if (frameCount % 2 == 0) {  
  
  /*
  if (keyPressed){
    if (key == ESC){
      exit();
    }
  }
  */
  

  fill(255, 0, random(255));
  pushMatrix();
  translate(400, 400);
  rotate(radians(rotate_v));
//  scale(scale_v);
  pen_stroke(de_po.x, de_po.y);
  
  rotate_v = rotate_v + random(-3.5, 3.5);
 // scale_v = scale_v - 0.0026;
 
  if (random(4) > 3.5){
  de_po.x = de_po.x + random(-de_acc.x, de_acc.x);
  de_po.y = de_po.y + random(-de_acc.y, de_acc.y);
  } 
  popMatrix();
}
  
}

void pen_stroke(float a, float b){
    maxWid = 30;
    currentWid = maxWid;
    for (int leng = 0; leng < random(0, 800); leng++){
      for (int wid = 0; wid < random(maxWid); wid++){
         if (random(4) > 1.5){
           noFill();
         }
         else if (random(4) < 1){
           //  fill(255, random(255), 3);
             //orange and red
           }
         else{
           fill(0, random(255), random(129, 255), random(50));
           //blue and pink
         }
          circle(a + wid, b + leng, 1);
          currentWid = wid;
      }
    }
}
