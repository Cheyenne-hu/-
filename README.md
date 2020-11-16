# -
float x1=0;
float y1;
float x2;
float y2;
float a=0;
float b=0;
float c=0;

void setup(){
size(800,800);
background(255);
colorMode(RGB,176,224,230);
frameRate(188);
}

void draw(){
x1=map(sin(a),-1,1,30,width-30);
y1=map(cos(a),-1,1,30,height-30);
x2=map(sin(b),-1,1,20,width-20);
y2=map(cos(b),-1,1,20,height-20);
stroke(c,100,60,10);
line(x1,y1,x2,y2);
a=a+0.01;
b=b+0.02+cos(b)/120;
c=c+0.005;
}
