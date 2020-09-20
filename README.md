# hw2_ExploringObjects-Arrays
Computational Practice 2


Question 1:
var people = [
  {
    name: "J.D. Zamfirescu",
    food: "宫保鸡丁",
    color: "blue"
  },
  {
    name: "Adam Smith",
    food: "小笼包",
    color: "red"
  },
  
  {
    name: "Sarah",
    food: "tofu",
    color: "black"
  },
  
  {
    name: "Chloe",
    food: "beans",
    color: "yellow"
  }

  
  
];

textAlign(CENTER);

for (var i = 0; i < people.length; i += 1) {
  fill(0);
  textSize(15);
  text("❤️", width/2, height/2-10);
  textSize(40);
  text(people[i].name, width/2, height/2-30);
  fill(people[i].color);
  text(people[i].food, width/2, height/2+30);
}

Question2:

var people = [
  {
    name: "J.D. Zamfirescu",
    food: "宫保鸡丁",
    color: "blue"
  },
  {
    name: "Adam Smith",
    food: "小笼包",
    color: "red"
  },
  
  {
    name: "Sarah",
    food: "tofu",
    color: "black"
  },
  
  {
    name: "Chloe",
    food: "beans",
    color: "yellow"
  }

  
  
];

textAlign(CENTER);

size= 10 
  var y= height/5 
for (var i = 0; i < people.length; i += 1) {
  fill(0);
  textSize(10);
	

  text("❤️", width/2, y);
  text(people[i].name, width/2, y-20);
  fill(people[i].color);
  text(people[i].food, width/2, y+20);
  y=y+100
 
}

Question 3:
var people = [
  {
    name: "J.D. Zamfirescu",
    food: "宫保鸡丁",
    color: "blue"
  },
  {
    name: "Adam Smith",
    food: "小笼包",
    color: "red"
  },
  
  {
    name: "Sarah",
    food: "tofu",
    color: "black"
  },
  
  {
    name: "Chloe",
    food: "beans",
    color: "yellow"
  }

  
  
];

textAlign(CENTER);

size= 10 
  var y= height/5 
for (var i = 0; i < people.length; i += 1) {
  fill(0);
  textSize(size);
	

  text("❤️", width/2, y);
  text(people[i].name, width/2, y-20);
  fill(people[i].color);
  text(people[i].food, width/2, y+20);
  y=y+100
  size=size+3
}

Optional Challenge 4:

var people = [
{
    name: "J.D. Zamfirescu",
    food: "宫保鸡丁",
    color: "blue"
  },
  {
    name: "Adam Smith",
    food: "小笼包",
    color: "red"
  },
  {
    name: "Sarah",
    food: "tofu",
    color: "black"
  },

  {
    name: "Chloe",
    food: "beans",
    color: "yellow"
  }

]

var emoji1 = "❤️";
var emoji2 = "💖";

var emoji = emoji1;



function setup() {
  createCanvas(400, 400);

  //   emojilayer = createGraphics(400, 400)
  //   emojilayer.background(255)
  background(255)
}

function draw() {
  textAlign(CENTER);
  size = 10

  var y = height / 5 // initial y
  for (var i = 0; i < people.length; i += 1) {
    fill(0);
    textSize(size)
    text(emoji, width / 2, y);
    text(people[i].name, width / 2, y - 20);
    fill(people[i].color);
    text(people[i].food, width / 2, y + 20);
    y = y + 100
    size = size + 3

  }

}

function mousePressed() {
  //do the swap of the hearts


  if (mouseIsPressed) {
    emoji = emoji2;
  } else {
    emoji = emoji1;
  }

}
