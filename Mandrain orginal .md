function setup() {
  createCanvas(300, 300);
}

function draw() {
  var lineX1 =20;
  var lineX2 =150;
  var lineX3 =240;
  var lineX4 =280;
  var lineX5 =350;
  var lineY1 =50;
  var lineY2 =90;
  var lineY3 =200;
  var lineY4 =250;
  
  background(250);
  noStroke();
  strokeCap(SQUARE);
  
  fill(250,255,0);//top yellow
  rect(0,0,lineX1,lineY1);// yellow rectangle
  
  fill(220,0,0);//top red
  rect(lineX2,0,lineX3-lineX2,lineY1);// red rectangle
  
  fill(220,0,0);//middle red
  rect(lineX1,lineY1,lineX2-lineX1,lineY3-lineY1);//red rectangle
  
  
  fill(250,255,0);//top yellow
  rect(lineX5,0,width-lineX5,lineY2);// yellow rectangle
  
  fill(0,120,255);// middle blue
  rect(lineX4,lineY1,lineX5-lineX4,lineY2-lineY1);///blue rectangle
  
  fill(250,255,0);//middle yellow
  rect(lineX3,lineY1,lineX4-lineX3,lineY4-lineY1);// yellow rectangle
  
  fill(0,120,255);// bottom blue
  rect(0,lineY3,lineX1,height-lineY3);///blue rectangle
  
  fill(220,0,0);//bottom red
  rect(lineX4,lineY4,width-lineX4,height-lineY4);// red rectangle
  
  stroke(0);//draw black
  strokeWeight(5);
  line(lineX3,lineY2,width,lineY2);  // vertical line2
	line(lineX1,0,mouseX,mouseY);//left horizonal line 1
  line(lineX2,0,mouseX,mouseY);//left horizonal line 2
  line(lineX3,0,mouseX,mouseY);// horizonal line 3
  line(lineX4,0,mouseX,mouseY);//horizonal line 4
  line(lineX5,0,mouseX,mouseY);
 
		
	strokeWeight(15); 
  line(0,lineY1,lineX5,lineY1);  // vertical line1
	
  strokeWeight(10); 
  line(0,lineY4,lineX1,lineY4);//vertical line4
  line(0,lineY3,lineX3,lineY3);// vertical line3
  line(lineX3,lineY4,width,lineY4); // vertical line5

}
