
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

 Doesn't work :/

```javascript

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

  guessthismakesthecolorrandomthatscool[anything1] = random(0, 255);
  wowanothercolorchannel[anything2] = random(0, 255);
  okonemoremaybe[anything3]=random(0, 255);

}

function draw() {
  background(180);

  for (let i = 0; i < numCircles; i++) {
    rect(idontknow[0], idontknow[1], idontknow[2], idontknow[3])
    fill(guessthismakesthecolorrandomthatscool[0], wowanothercolorchannel[1], okonemoremaybe[2]);


  }
}

```
