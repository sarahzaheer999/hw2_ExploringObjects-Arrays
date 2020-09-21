# Exploring-Objects-and-Arrays 
Done in rudy.zamfi.net and p5edior(optional challenge); By Chloe Kim and Sarah Zaheer


### Add two more "people" object literals to the people array
```
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
    food: "cake",
    color: "pink"
  },
  
  {
    name: "Chloe",
    food: "rice",
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
```
### Fix the overlapping text issue by using the index variable i in the body of the for loop to modify the y coordinate of the drawn text.

#### One way of doing it 
```
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
    food: "cake",
    color: "pink"
  },
  
  {
    name: "Chloe",
    food: "rice",
    color: "yellow"
  }

  
  
];

textAlign(CENTER);

for (var i = 0; i < people.length; i += 1) {
  fill(0);
  textSize(15);
  clear ()
  text("❤️", width/2, height/2-10);
  textSize(40);
  text(people[i].name, width/2, height/2-30);
  fill(people[i].color);
  text(people[i].food, width/2, height/2+30);
}
```
#### Another way of doing it:-
```
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
    food: "cake",
    color: "pink"
  },
  
  {
    name: "Chloe",
    food: "rice",
    color: "yellow"
  }

  
  
];

textAlign(CENTER);

size= 10 
  var x= height/15
for (var i = 0; i < people.length; i += 1) {
  fill(0);
  textSize(10);
	

  text("❤️", width/3, x-5);
  text(people[i].name, width/2, x-10);
  fill(people[i].color);
  text(people[i].food, width/2, x+10);
  x=x+100
 
}

```
### Add a property to all objects for size; use it to change the font size of each person's words.
```
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
    food: "cake",
    color: "pink"
  },
  
  {
    name: "Chloe",
    food: "rice",
    color: "yellow"
  }

  
  
];

textAlign(CENTER);

size= 10 
  var x= height/10  
for (var i = 0; i < people.length; i += 1) {
  fill(0);
  textSize(10);
	

  text("❤️", width/5, x-5);
  textSize(size);
  text(people[i].name, width/2, x-10);
  fill(people[i].color);
  text(people[i].food, width/2, x+20);
  x=x+80
  size=size+8
}


```



### Optional Challenge 5:

```
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
```
