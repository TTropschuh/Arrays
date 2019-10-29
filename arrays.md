
# Arrays

## Random rectangles

```javascript

let numCircles = 10;
idontknow = [];

function setup() {
  createCanvas(600, 400);

  for (let i = 0; i < numCircles; i++) {
    idontknow[i] = random(0,400);
  }
}

function draw() {
  background(180);
  for (let i = 0; i < numCircles; i++) {
    rect(idontknow[0], idontknow[1],idontknow[2], idontknow[3])


  }
}

```
## Random rectangles that get even more random! Wow!


```javascript

// This sketch well let the rectangles change in size and color everytime it is refreshed.

let numCircles = 10;
idontknow = [];
guessthismakesthecolorrandomthatscool = [];
wowanothercolorchannel = [];
okonemoremaybe = [];

function setup() {
  createCanvas(600, 400);

  for (let i = 0; i < numCircles; i++) {
    idontknow[i] = random(0, 400);
  }

  let anything1 = 0;
  let anything2 = 0;
  let anything3 = 0;

}

function draw() {
  background(180);
let colorR = random(0,255);
  let colorG = random(0,255);
  let colorB = random(0,255);

  for (let i = 0; i < numCircles; i++) {
    rect(idontknow[0], idontknow[1], idontknow[2], idontknow[3])
    fill(colorR, colorG, colorB );

    noLoop();



  }
}

```

## Randomly colored/sized circles

```javascript
let diameters = [];
let posX = [];
let posY = [];
let colorred = [];
let colorgreen = [];
let colorblue = [];


function setup() {
  createCanvas(600, 400);
  background(200);


  // Amount of circles
  let numCircles = 10;
  for (let i = 0; i < numCircles; i++) {
    colorred[i] = floor(random(0, 255));
    colorgreen[i] = floor(random(0, 255));
    colorblue[i] = floor(random(0, 255));
    diameters[i] = random(10, 50);
    posX[i] = random(50, 550);
    posY[i] = random(50, 350);
  }


}

function draw() {

  drawcircles();

}


function drawcircles() {

  //
  for (let i = 0; i < diameters.length; i++) {
    fill(colorred[i], colorblue[i], colorblue[i]);
    circle(posX[i], posY[i], diameters[i]);

    noLoop();

  }
}
```

## My own idea

```javascript
let point1 = [];
let point2 = [];


function setup() {
  createCanvas(400, 400);


}

function draw() {
  background(220);

  drawLines1();


  noLoop();



}

function drawLines1() {
  let numLines = 10;
  for (let i = 0; i < numLines; i++) {
    point1[i] = random(50, 350);
    point2[i] = random(50, 350);

    line(point1[i], point2[i], point2[i], point1[i]);



    if (point1[i] > width/2){
   circle(point1[i],point2[i],10);
    }
    
     if (point1[i] < width/2){
   circle(point1[i],point2[i],10);
    }
  }
  print(point1);
    print(point2);

}
```
