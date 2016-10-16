# Projection_Mapping_Test

// RTA_948_ProjectionMapping Sketch

import deadpixel.keystone.*;
import processing.video.*;

Movie myMovie;

Keystone ks;
CornerPinSurface surface;
CornerPinSurface surface2;
CornerPinSurface surface3;
CornerPinSurface surface4;
CornerPinSurface surface5;
CornerPinSurface surface6;
CornerPinSurface surface7;
CornerPinSurface surface8;
CornerPinSurface surface9;
CornerPinSurface surface10;
CornerPinSurface surface11;
CornerPinSurface surface12;

PGraphics offscreen;
PGraphics offscreen2;
PGraphics offscreen3;
PGraphics offscreen4;
PGraphics offscreen5;
PGraphics offscreen6;
PGraphics offscreen7;
PGraphics offscreen8;
PGraphics offscreen9;
PGraphics offscreen10;
PGraphics offscreen11;
PGraphics offscreen12;

void setup() {
  fullScreen(P3D);

  ks = new Keystone(this);
  surface = ks.createCornerPinSurface(600, 350, 10);
  
  surface2 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface3 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface4 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface5 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface6 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface7 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface8 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface9 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface10 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface11 = ks.createCornerPinSurface(600, 350, 10); 
  
  surface12 = ks.createCornerPinSurface(600, 350, 10); 
  
  offscreen = createGraphics(width, height, P2D);
  offscreen2 = createGraphics(width, height, P2D);
  offscreen3 = createGraphics(width, height, P2D);
  offscreen4 = createGraphics(width, height, P2D);
  offscreen5 = createGraphics(width, height, P2D);
  offscreen6 = createGraphics(width, height, P2D);
  offscreen7 = createGraphics(width, height, P2D);
  offscreen8 = createGraphics(width, height, P2D);
  offscreen9 = createGraphics(width, height, P2D);
  offscreen10 = createGraphics(width, height, P2D);
  offscreen11 = createGraphics(width, height, P2D);
  offscreen12 = createGraphics(width, height, P2D);
  
  myMovie = new Movie(this, "Triangle_Explosive.mov");
  myMovie.loop();
}

void draw() {
  if (myMovie.available() == true) {
    myMovie.read();
  }  

  float md = myMovie.duration();
  float mt = myMovie.time();

  offscreen.beginDraw();
  offscreen.smooth();
  offscreen.strokeWeight(5);
  offscreen.fill(255,200,100,100);    
  offscreen.background(0);  
  offscreen.image(myMovie, 0, 0);  
  offscreen.endDraw();  
  
  offscreen2.beginDraw();
  offscreen2.smooth();
  offscreen2.strokeWeight(5);
  offscreen2.fill(255,200,100,100);    
  offscreen2.background(0);  
  offscreen2.image(myMovie, 0, 0);  
  offscreen2.endDraw();  
  
  offscreen3.beginDraw();
  offscreen3.smooth();
  offscreen3.strokeWeight(5);
  offscreen3.fill(255,200,100,100);    
  offscreen3.background(0);  
  offscreen3.image(myMovie, 0, 0);  
  offscreen3.endDraw();  
  
  offscreen4.beginDraw();
  offscreen4.smooth();
  offscreen4.strokeWeight(5);
  offscreen4.fill(255,200,100,100);    
  offscreen4.background(0);  
  offscreen4.image(myMovie, 0, 0);  
  offscreen4.endDraw();  
  
  if (mt > md/2.0) {
  
  offscreen5.beginDraw();
  offscreen5.smooth();
  offscreen5.strokeWeight(5);
  offscreen5.fill(255,200,100,100);    
  offscreen5.background(0);  
  offscreen5.image(myMovie, 0, 0);  
  offscreen5.endDraw();  
  
  offscreen6.beginDraw();
  offscreen6.smooth();
  offscreen6.strokeWeight(5);
  offscreen6.fill(255,200,100,100);    
  offscreen6.background(0);  
  offscreen6.image(myMovie, 0, 0);  
  offscreen6.endDraw();  
  
  offscreen7.beginDraw();
  offscreen7.smooth();
  offscreen7.strokeWeight(5);
  offscreen7.fill(255,200,100,100);    
  offscreen7.background(0);  
  offscreen7.image(myMovie, 0, 0);  
  offscreen7.endDraw();  
  
  offscreen8.beginDraw();
  offscreen8.smooth();
  offscreen8.strokeWeight(5);
  offscreen8.fill(255,200,100,100);    
  offscreen8.background(0);  
  offscreen8.image(myMovie, 0, 0);  
  offscreen8.endDraw();  
  
  if (mt > md/4.0) {
  
  offscreen9.beginDraw();
  offscreen9.smooth();
  offscreen9.strokeWeight(5);
  offscreen9.fill(255,200,100,100);    
  offscreen9.background(0);  
  offscreen9.image(myMovie, 0, 0);  
  offscreen9.endDraw();  
  
  offscreen10.beginDraw();
  offscreen10.smooth();
  offscreen10.strokeWeight(5);
  offscreen10.fill(255,200,100,100);    
  offscreen10.background(0);  
  offscreen10.image(myMovie, 0, 0);  
  offscreen10.endDraw();  
  
  offscreen11.beginDraw();
  offscreen11.smooth();
  offscreen11.strokeWeight(5);
  offscreen11.fill(255,200,100,100);    
  offscreen11.background(0);  
  offscreen11.image(myMovie, 0, 0);  
  offscreen11.endDraw();  
  
  offscreen12.beginDraw();
  offscreen12.smooth();
  offscreen12.strokeWeight(5);
  offscreen12.fill(255,200,100,100);    
  offscreen12.background(0);  
  offscreen12.image(myMovie, 0, 0);  
  offscreen12.endDraw(); 
  
  }
  }
  background(0);
  
  surface.render(offscreen);
  surface2.render(offscreen2);
  surface3.render(offscreen3);
  surface4.render(offscreen4);
  surface5.render(offscreen5);
  surface6.render(offscreen6);
  surface7.render(offscreen7);
  surface8.render(offscreen8);
  surface9.render(offscreen9);
  surface10.render(offscreen10);
  surface11.render(offscreen11);
  surface12.render(offscreen12);
}


void keyPressed() {

  switch(key) {
  case 'c':
    // enter/leave calibration mode, where surfaces can be warped 
    // & moved
    ks.toggleCalibration();
    break;

  case 'l':
    // loads the saved layout
    ks.load();
    break;

  case 's':
    // saves the layout
    ks.save();
    break;
  }  
}
