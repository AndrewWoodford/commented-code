int num = 100; //determines the size of the object
float mx[] = new float[num];
float my[] = new float[num];

void setup() { //"allows you to set it up"
  size(640, 360); //changes the size of the window it pulls open
  noStroke(); //removes the lines a round the circles
  fill(255, 153); //changes the color of the object 
}

void draw() { //executes the lines of code in its block
  background(1000); //changes the background color
  
  // Cycle through the array, using a different entry on each frame. 
  // Using modulo (%) like this is faster than moving all the values over.
  int which = frameCount % num;
  mx[which] = mouseX; // makes the dot follow the mouse on the y axis
  my[which] = mouseY; //makes the dot follow the mouse on the y axis
  
  for (int i = 0; i < num; i++) {
    // which+1 is the smallest (the oldest in the array)
    int index = (which+1 + i) % num;
    rect(mx[index], my[index], i, i);  //determines the shape of the object
  }
}
