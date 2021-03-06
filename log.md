# 100 Days Of Code - Log


###  Day 93: Sunday May 14, 2017
#####

**Today's Progress**: Restarted the lab again and was able to solve a few lines of code. I was confused by an if statement where i was supposed to follow some instructions because it started with if {false ...instructions... return true}. That bugged me for a while, I finally asked a question and they told me that I could remove that, that I needed to check for the conditions in the instructions and if they pass/fail it should return true.

**Thoughts**: Bummer... my confindence is low right now. Now I'm questioning whether online learning is really for me, after I've decided to take the online course.


1. [Today's tweet](https://twitter.com/catespinosa/status/863943924502728705)



###  Day 92: Saturday May 13, 2017
#####

**Today's Progress**: Started on the last exercise of the JS track on learn.co "Rock Dodger". I'm supposed to create the functions that will move the dodger to avoid the rocks. I did not get very far at all. I also found out that in order to preview and HTML file from the labs, I had to run httpserver which would allow me to view the file in the browser.

**Thoughts**: This is when it gets hard. I'm a little discouraged because I don't know where to even begin with this.

1. [Today's tweet](https://twitter.com/catespinosa/status/863600699963256832)




###  Day 91: Friday May 12, 2017
#####

**Today's Progress**: implementing event listeners and practiced updating an object's position on the page

		Define a function getIt that does not accept a parameter. The function should bind a click event to the p tag. When the paragraph is clicked, the function should alert "Hey!".

		Define a function frameIt that does not accept a parameter. The function should bind the load event that adds the class tasty to the image to add a red frame to the image.

		Define a function pressIt that does not accept a parameter. The function should bind a keydown event to the input field of the form that alerts a user when they have pressed the G key.

		Define a function submitIt that does not accept a parameter. The function should bind a submit event to the form that alerts "Your form is going to be submitted now.".


**Thoughts**: 

1. [Today's tweet](https://twitter.com/catespinosa/status/863224124268838912)




###  Day 90: Thursday May 11, 2017
#####

**Today's Progress**: Finally jQuery exercises. Modifying HTML with jQuery and selectors.


**Thoughts**: 

1. [Today's tweet](https://twitter.com/catespinosa/status/862887042249871360)


###  Day 89: Wednesday May 10, 2017
#####

**Today's Progress**: Further reading on bubbling and capturing. Learned about
	event.detail - tells you how many times the mouse was clicked in the same area
	event.which - which keyboard key was pressed

I completed the [Konami Code Lab](https://learn.co/tracks/bootcamp-prep/javascript-fundamentals/the-dom/konami-code-lab) to practice event listeners. I need to read up on parseInt() because I don't quite understand it.

		const code = [38, 38, 40, 40, 37, 39, 37, 39, 66, 65]

		function init() {
		  // your code here
		  //You'll want to attach an event listener to document.body and check for 'keydown' events.
		  //If the user enters this special code, alert() a congratulatory message.
		  //But if they start entering anything else anywhere along the way, don't trigger anything out of the ordinary.
		  //When you're testing the code out, be sure to call init() to set everything up!

		  let index = 0;
		  const body = document.body;


		  body.addEventListener('keydown', function(e){
		    const key = parseInt(e.detail || e.which)
		    if (key === code[index]) {
		      index++

		      if (index === code.length - 1) {
		        alert('You pressed the right key!')
		        index = 0
		      }
		    }
		      else {
		        index = 0
		      }
		    })
		}
		    init ();


**Thoughts**: 

1. [Today's tweet](https://twitter.com/catespinosa/status/862516213993418753)


###  Day 88: Tuesday May 9, 2017
#####

**Today's Progress**: Reading about DOM Nodes, Callbacks.

Callbacks are functions that are passed as arguments in other functions. Listening to Nodes
		addEventListener() takes two arguments. The name of the event and a function to handle the event.

	Preventing default behavior:
		preventDefault()
		stopPropagation() interrupts the event's normal behavior. I'm not seeing the difference between these two.

DOM events propagate by bubbling (starting at the target node and moving up the DOM tree to the root - I even drew an upside down tree in my notebook)

They also propagate by capturing - starting form the target node's parent and propagating down the tree until it reaches the target.

Events bubble by default

**Thoughts**: Started taking notes and I feel more confident in what I'm learning, and more motivated to learn.

1. [Today's tweet](https://twitter.com/catespinosa/status/862117393660817408)



###  Day 87: Monday May 8, 2017
#####

**Today's Progress**: [Hide and Seek Lab is up on github](https://github.com/catespinosa/javascript-hide-and-seek-bootcamp-prep-000/blob/master/index.js)

**Thoughts**:Reviewed CSS selectors or rather learned what to call them. It's incredible that I have been working with CSS for so many years and didn't know what to call them exactly. Shame!!

1. [Today's tweet](https://twitter.com/catespinosa/status/861783544447762432)



###  Day 86: Thursday May 4, 2017
#####

**Today's Progress**: Reviewed yesterday's lesson on traversing objects, exploring the DOM as a tree CS

1. [Today's tweet](https://twitter.com/catespinosa/status/860340209292070912)



###  Day 85: Wednesday May 3, 2017
#####

**Today's Progress**: Read .@learn_co lesson on Traversing Nested Objects and Breadth-first search.

1. [Today's tweet](https://twitter.com/catespinosa/status/860148078380187649)


###  Day 83-84: Monday May 1 - Tuesday May 2, 2017 
#####

**Today's Progress**: Between Monday and Tuesday, I worked on this exercise. It shouldn't have taken this long but my ability to concentrate lately is very low.

1. Define a function `viewCart` which does not accept any arguments. This function should loop over every item in `cart` to print out `"In your cart, you have [item and price pairs]."`. If there isn't anything in your cart, the function should print out `"Your shopping cart is empty."`

* The first part called for an if-else statement. If the cart is empty or === 0 then console log that the cart is empty.
* Else, I need to loop through the items and print out each one in item/price pairs.

My code looks like this:

		function viewCart() {
		  if(cart.length === 0) {
		    console.log("Your shopping cart is empty.")
		  } else {
		    var items = [];
		    for (var i = 0; i < cart.length; i++) {
		      for (var price in cart[i]) {
		        items.push(`${price} at $${cart[i][price]}`)
		      }
		    }
		    console.log(`In your cart, you have ${items.join(", ")}.`)
		  }
		}



2. Define a function `removeFromCart` which accepts one argument, the name of the item you wish to remove. If the item isn't in the cart, the function should print out `"That item is not in your cart."`. If the item is in your cart, it should remove the object from the `cart` array. Then return the cart. (**HINT**: Check each object's key to see if it matches the parameter, then remove it if it matches. You might find [hasOwnProperty](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty) to be useful.)

Here's the code:
		function removeFromCart(item) {
		  let iHaveIt = false

		  for (let i = 0; i < cart.length; i++) {
		    if (cart[i].hasOwnProperty(item)) {
		      iHaveIt = true
		      cart = cart.slice(0, i)
		      }
		    }
		  if (iHaveIt === false) {
		    console.log("That item is not in your cart.")
		  }
		 return cart
		}


3. Define a function `placeOrder` which accepts one argument, a credit card number. If no argument is received, then the function should print out `"We don't have a credit card on file for you to place your order."`. If there is a credit card on file, the function should print out `"Your total cost is $${total()}, which will be charged to the card ${cardNumber}."`. The function should empty the `cart` array.

		function placeOrder(cardNumber) {
		  if (cardNumber === undefined) {
		  console.log("We don\'t have a credit card on file for you to place your order.")
		} else {
		  console.log(`Your total cost is $${total()}, which will be charged to the card ${cardNumber}.`)
		  cart = [];
		}
		return cart
		}
		


1. [Today's tweet](https://twitter.com/catespinosa/status/859580348774191104)


###  Day 82: Sunday April 30, 2017 
#####

**Today's Progress**:

Started the online shopping lab and finished the first problem:

* Define a global variable (use var at the top level) called cart. Initialize it as an empty array.
* Define a function getCart that takes no arguments and returns the cart.
* Define a function addToCart. This function should accept one argument, the item the user wants to purchase.
This function should automatically set a price for this item by generating a random number between 0 and 100. (Hint: Math.random() generates a random number in 0, 1; Math.floor() rounds a number down to the nearest integer.)
This function should add the item and the price as an object ({item: price}) to the cart array. This function should print out to the console <item> has been added to your cart. and return the cart.

So I defined "price" as a variable to execute Math.floor((Math.random() * 100) + 1). Then I defined the newItemPrice variable to create the object {item : price} and push it into the cart array. The next step called for a console log (`${item} has been added to your cart.`) and finally return the cart array.

My code looks like this:

		var cart = [];

		function addToCart (item) {
			var price = Math.floor((Math.random() * 100) + 1);
			var newItemPrice =  {item : price};
			cart.push(newItemPrice);
			console.log(`${item} has been added to your cart.`);
			return cart;
		}

More on this exercise tomorrow.


1. [Today's tweet](https://twitter.com/catespinosa/status/858811905359663104)



###  Day 81: Friday April 28, 2017 
#####

**Today's Progress**: Lesson 29 in learn.co bootcamp prep: Add elements to an array. Return items from an array. Iterate through an array. Pass an array as a function parameter

1. [Today's tweet](https://twitter.com/catespinosa/status/858168843956617216)


###  Day 80: Thursday April 27, 2017 
#####

**Today's Progress**: Went back to learn.co's bootcamp prep. I'm up to lesson 28 and it was extremely difficult to switch gears from CSS and not practicing javascript to this lesson. OMG. I have to pick a topic and stick to it, but I'm glad I'm figuring out how to best approach this challenge.

1. [Today's tweet](https://twitter.com/catespinosa/status/857796717386883072)



###  Day 79: Wednesday April 26, 2017 
#####

**Today's Progress**: Finished CSS Grid Garden. I was having a hard time splitting the garden according to the instructions or rather I wasn't understanding the instructions. finally I reached out to someone on twitter who helped me figured it out.  The question was asking to split the garden into two rows - one big one at the top, and then the 50px path at the bottom. I had split it into 3 rows.

I'm hoping my reading comprehension gets better or rather I think I've been extremely distracted this past week and it's been that much harder to concentrate and understand instructions.


1. [Today's tweet](https://twitter.com/catespinosa/status/857326795452022785)


###  Day 78: Tuesday April 25, 2017 
#####

**Today's Progress**: Moved up 2 levels up to the last level of css grid garden and got stuck again.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/857070407857393665)



###  Day 77: Monday April 24, 2017 
#####

**Today's Progress**: Started CSS Grid Garden. Breezed through most of the levels until I got stuck on level 26


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/856695770946437120)


###  Day 76: Sunday April 23, 2017 
#####

**Today's Progress**: Continued on css grid exercise from day 73 but couldn't make the layout response.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/856331448374222849)


###  Day 74-75: Friday April 21-22, 2017 
#####

**Today's Progress**: Attended Codeland Conference. The two day event was an awesome experience. I don't know if it qualifies as progress but I'm going with it :)

The talks were not too technical but gave you a peek into the life of a developer, provided tools on how to deal with failure, mental health issues, and a roadmap on how to get the career you want.

I was very happy with the experience, there was definitely a sense of community and camaraderie in the room. Everyone was super nice, the speakers were engaging and I couldn't have asked for more. I am really glad that I went.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/856331118387351556)




###  Day 73: Thursday April 20, 2017 
#####

**Today's Progress**: Worked on text overlap with grid based on jenn simmons labs. Looked into object-fit CSS property since the lab uses object-fit: cover. It'll fill in the element's box maintaining its aspect ratio. I'm working with a rectangular image, so it shows part of it but it didn't distort the dimensions.

fill
The replaced content is sized to fill the element’s content box: the object’s concrete object size is the element’s used width and height.

contain
The replaced content is sized to maintain its aspect ratio while fitting within the element’s content box: its concrete object size is resolved as a contain constraint against the element’s used width and height.

cover
The replaced content is sized to maintain its aspect ratio while filling the element’s entire content box: its concrete object size is resolved as a cover constraint against the element’s used width and height.

none
The replaced content is not resized to fit inside the element’s content box: the object’s concrete object size is determined using the default sizing algorithm with no specified size, and a default object size equal to the replaced element’s used width and height.


**Link to work:** 

1. [Grid folder - overlap](https://github.com/catespinosa/catespinosa.github.io/commit/375431198fe85deb129461df28888b1999f38b20#diff-585e6efefe03616bc439bd901e93f89e)

2. [Today's tweet](https://twitter.com/catespinosa/status/855041562224590849)



###  Day 64-72: Friday April 7 - Wednesday April 19, 2017 
#####

**Today's Progress**: I have not kept up with updating the log obviously but I've continued to post on Twitter. I've published my portfolio at catherineespinosa.com and decided to use squarespace so that I can easily add content. However, I'm not too happy with the platform and it makes me want to handcode again.

**Thoughts**: I've put too much pressure on getting projects done, but I'm happy at least I brought my domain back. Building portfolio worthy pieces will take me some time and experimenting. So far I only have work stuff, if that. I've skipped days since last time I posted because I went away for Easter.



###  Day 64: Thursday April 6, 2017 
#####

**Today's Progress**: Finally started using Grid. I looked into different column and row spans, found out how to target the children of an element: I thought I wasn't going to be able to do it with a div, but I was able to target the children of the #portfolio div which is AWESOME! I can make the cards different sizes. I will have to use CSS feature queries (@supports (property:value)) for browsers that support Grid, then I will have to specify styles for other browsers and use floats with specific width etc.

**Thoughts**: 


###  Day 63: Wednesday April 5, 2017 
#####

**Today's Progress**: Started laying out the image cards to display my work, copied a hover effect from https://miketricking.github.io/bootstrap-image-hover/ and will be editing that tomorrow. Placing the thumbnails on the page really makes me want to start using grid and I think I'm just going to do that tomorrow.

**Thoughts**: Since Grid won't get out of my head, I'm going to start using it tomorrow.

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/849822898906947584)


###  Day 62: Tuesday April 4, 2017 
#####

**Today's Progress**: Continued to work on my portfolio. Added a photo which makes it look like a LinkedIn profile, added some colors but not sure if that's what I'm going to end up with. I think to keep it simple I will go with a standard format which is big hero header, then three columns for the portfolio pieces. Added a fixed nav also.

**Thoughts**: Trying really hard not to use a framework. I'm getting ideas from Bootstrap and Squarespace sites but I'd like to continue to use my own code. I also might use jQuery for adding portfolio pieces... I thought I said I wanted to keep it simple = make my life easier? But I think I have a good idea about how to add thumbnails dynamically.

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/849457452642959360)



###  Day 61: Monday April 3, 2017 
#####

**Today's Progress**: More like Tuesday... Went over my work for an idea of what I want to put up on my portfolio, I have a vague idea of what I want my portfolio to look like. Started from scratch with my html and css files in an attempt not to use a framework AKA same way I've always worked. Played around with viewport units with CSS to change the size of the header and also made the header the height of the viewport. Interesting concept. I may add a photo later. I'll be designing in the browser.

**Thoughts**: Going over my work was tough but it is what it is. I want to work on my portfolio and continue to build more sites so that I can refresh what I've already done.

**Link to work:** 

1. [Viewport units experiment on portfolio](https://github.com/catespinosa/catespinosa.github.io/commit/70d0a330443710c2826f4b7ab62c00d36b4d4130)

2. [Today's tweet](https://twitter.com/catespinosa/status/849131813893136386)



###  Day 59-60: Saturday and Sunday April 1 - 2, 2017 
#####

**Today's Progress**: Continued to do more research and planning. Watched “Modern Layouts: Getting Out of Our Ruts by Jen Simmons". That talk was so eye opening. I had already heard her talk about how web design doesn't have to look the same, but hearing it again makes me look at websites in such a different way! 

**Thoughts**: I didn't do any coding and I know it's because I'm putting it off... I just have to get started somewhere. What I start with doesn't have to dictate how the final product is going to look like, when does it ever?

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/848739286354669568)

###  Day 58: Friday March 31, 2017 
#####

**Today's Progress**: Planning my portfolio. I want to use CSS Grid

**Thoughts**: Since I have more time to code on the weekends, I'm going to dedicate the weekends to work on my portfolio and weekdays to do labs. I almost go to sleep without coding but I felt guilty so here I am past midnight (it's still March 31st in California). I sketched my ideas so let's see how I do. I also looked at squarespace after and thought "why not?" but somehow I feel like I shouldn't... plus squarespace is way too pretty for my stuff. LOL. Imposter!!

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/848039341913976833)

###  Day 57: Thursday March 30, 2017 
#####

**Today's Progress**: Learn.co for loop, while loop, do-while loop. 

**Thoughts**: I've never done a do-while loop or a while loop. Lab was kind of tricky and I was pissed I couldn't figure it out.

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/847614919847460865)


###  Day 56: Wednesday March 29, 2017 
#####

**Today's Progress**: Finished the Grid exercises from the workshop I attended on Saturday. Started for loops lab on learn.co.

**Thoughts**: I have to start working on something in order to understand it, then I read about it so it can sink in. I can't believe I just said that. I just decoded my learning style. 


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/847281390462709760)
2. [Codepen exercise 11](http://codepen.io/catespinosa/pen/XMygZw)
3. [Codepen exercise 10](http://codepen.io/catespinosa/pen/QpJgvm)


###  Day 55: Monday March 27, 2017 
#####

**Today's Progress**: Practiced CSS Grid again on Codepen

**Thoughts**: Still trying to understand it.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/846534819878227968)
2. [Codepen exercise 8](http://codepen.io/catespinosa/pen/aJaRBQ)
3. [Codepen exercise 9](http://codepen.io/catespinosa/pen/BWOqwp)


###  Day 54: Sunday March 26, 2017 
#####

**Today's Progress**: Learn.co Javascript Objects labs. Learned to use Object.assign()

**Thoughts**: 


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/846195371097444353)


###  Day 53: Saturday March 25, 2017 
#####

**Today's Progress**: Went to the CSS Grid workshop with Jen Simmons at General Assembly. Practice with the lab examples provided by the host.

**Thoughts**: This past 7 months have been really eye opening. I feel like I have been living under a rock for 10 years because I was not actively seeking to update my web design skills or move onto web development. A lot of it has to do with the nature of my job since it's not a pure web design role but still, I feel like I could have done so much more. There's no point in having regrets so I can only look forward and what I'm willing to do now. This workshop was really inspiring as everything else that I have learned or seen during this 100 day challenge.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/845657775292235776)



###  Day 52: Friday March 24, 2017 
#####

**Today's Progress**: Continued on the bootcamp prep on @learn_co JavaScript arrays lab.

**Thoughts**: Same as the day before. Most of the learn.co stuff is ES6, so I'm learing something new while I complete these labs.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/845485985119064066)



###  Day 51: Thursday March 23, 2017 
#####

**Today's Progress**: Continued on the bootcamp prep on @learn_co JavaScript arrays lab.

**Thoughts**: I was confused by why the learn IDE app was passing my tests if the functions weren't correct. Basically I had two functions that were the same but they were supposed to be different, yet the app was saying they were both correct when one of them was clearly not. I asked a question and was quickly invited to do a screenshare with one of the instructors who helped me figure out that it was a bug in the system. So we went over how to update arrays non-destructively. I thought I passed the lab pretty quickly if it weren't for that bug that didn't allow me to move forward.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/845122228198899715)


###  Day 50: Wednesday March 22, 2017 
#####

**Today's Progress**: Worked on learn.co's hoisting lab. Since this is a bootcamp prep, I have to go over arrays again, but the app was not responding and it's too late. 

**Thoughts**: TODAY IS DAY 50!! I'm proud of myself for not giving up. I've skipped a few days in between but made sure to get right back on it. I've set 4 goals when I first started the challenge but I didn't complete them all and I had to move in a different order. At least I have a page to show for. I can read documentation and feel like I can understand and can work with it without feeling scared or like WTF all the time... I mean, I still do say WTF is this, but I don't give up and I get back to it: Look at all my posts about CORS (even though I didn't use it LOL). I've tried different approaches to learning: by doing and following online tutorials. I've also gone to meetups about coding!! I wouldn't have been able to gather up the confindence to do that a year ago (because I didn't know about this anyway haha)

**Things I need to work on**:
* By nature I am a procrastinator and disorganized, so I've been leaving the hour of code mostly for the night time because that's when I can "fit" it into my "schedule". I want to get more organized and set a specific time in which to code

* Still giving myself somewhat of a hard time over what others are working on. So I want to focus on what I'm learning and remind that I can only be a better version of myself. The good thing is that at least I'm not so clueless about code

*Read books

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/844757189428371456)



###  Day 49: Tuesday March 21, 2017 
#####

**Today's Progress**: completed the learn.co fix the scope lab. The first functions were easy but the last function was supposed to call a function within a function. So I tried to follow the example and asked questions but finally someone said I had to use two sets of parenthesis! Huh? I've never done that before. So even though I feel like I should already know this, I don't. I keep repeating myself LOL their material is hard.

**Thoughts**: Only put in 1 hour today because... LIFE

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/844378216739622912)


###  Day 48: Monday March 20, 2017 
#####

**Today's Progress**: Continued to work on my my dance project's CSS. FIxed the images for the header in PHotoshop. Changed the colors for the thumbnails you click on when you want to listen to the music. I also changed the nav bar color and made the whole site into a more cohesive unit. I was happy to get away from the Blue and REd of the Cuban flag. Played a lot with Bootstrap but decided to keep the same layout I had because I've spent way too much time on it and I need to move on. It's almost half way through the challenge and I think I should do some learning.

I need to delete a bunch of files that I pushed last night because I've been keeping them all in the same project folder ie. photoshop files etc... I will look into git ignore or move them this weekend.

**Thoughts**: I was nervous to share with the "World" or Twitter but this project made me realize that I need to work on quicker iterations. SInce I don't design full time for work my skills are rusty, and I also feel intimidated by the new standards. I know sites nowadays rely heavily on photos but I didn't want to put a photo as the first thing you saw, so that's why I decided to go in the direction i went in.

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/844046834393923586)
2. [Cuban music and dance project](catespinosa.github.io/jsd920_class_repo/projects/final_project/public/index.html)



###  Day 47: Sunday March 19, 2017 
#####

**Today's Progress**: Finished the arithmetic functions lab and took a quiz about functions on learn.co. I took a long time trying to figure out how to use the parseInt() function within a function. I was trying to return the argument that I was passing from my makeInt(n) function, but that kept giving me error because the parseInt returns a new value, not the argument that I'm passing which would remain unchanged if I just did - return n -. I had to look at the solution and it turns out I had to return parseInt function in order to pass the test.

I also worked on changing my dance project's CSS. Started with the header color and added 2 background images to the same element for the first time. I didn't know you could add different images as backgrounds.


**Thoughts**: Still not happy with the design and starting to feel like I'm not good enough and like I'm just doing thing the "old" way I know how to and start bringing myself down. 				

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/843609284827103232)


###  Day 46: Saturday March 18, 2017 
#####

**Today's Progress**: Skipped Friday's session because of a family event. Today I learned string interpolation and ES6 template literals in the learn.co functions lab on the bootcamp prep track.

**Thoughts**: I need to start working on my portfolio.  				

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/843159287430086656)



###  Day 45: Thursday March 16, 2017 (into March 17th)
#####

**Today's Progress**: Skipped 2 full days because of being extremely busy at work, extremely tired, and I also had a company event to attend yesterday. Today I finished the functions lab... GEESH!! Another difficult one, I was stumped on how to approach the problem. The problems said "IF the string is lowercase then do something" but my if statements kept FAILING!! I ended up hardcoding the values of the param but that was not the idea. I had to use toLowerCase(), toUpperCase()... when I did that I was getting "Expected undefined to equal 'I can\'t hear you!'", and it was because the syntax was wrong. I was missing the parenthesis next to the toUpper or Lower methods. I spent an hour getting errors.

**Thoughts**: 				

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/842589749692977152)



###  Day 44: Monday March 13, 2017 (into March 14th)
#####

**Today's Progress**: These labs are no joke. I thought I would breeze through them. Today I actually finished the Flow Control lab: if/else statements, switch statements. I think the tests have taken some getting used to and that's why I keep taking so long with the labs. Well I think I'm taking long but I only did 1 hour, I hope I get faster with time!

**Thoughts**: 				

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/841504686771445760)



###  Day 43: Sunday March 12, 2017
#####

**Today's Progress**: Continued learn.co bootcamp prep. Now on Javascript flow control

**Thoughts**: I've been working on the Free Code Camp challenges lately, and I thought that the learn.co platform would be similar, but it provides much more context for what you're trying to accomplish with your code. It provides a conversational approach to teaching code which I thoroughly appreciate because it feels like someone is actually teaching you. It still took me a while to get used to, which is why my day 41 and 42 were about the same thing. It took me a while to realize that I needed to install the IDE app on this computer (I've been using a new computer for the past month) in order to get the labs to work. The first part of these javascript labs were tests. I had to run the tests before writing any code, and that part was new even though I had taken a JS course before, but I was glad to work with them because it's something that I hadn't done before.  				

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/841386682960117761)


###  Day 41-42: Friday March 10 and Saturday March 11, 2017
#####

**Today's Progress**: learn.co bootcamp prep

**Thoughts**: I received wonderful news on Thursday. I've been awarded a partial scholarship to the Flatiron School's online web development program thanks to Women Who Code and the Flatiron School. So it was exciting and scary at the same time, am I going to really become a web developer? "You have to take advantage of an opportunity of a lifetime, in the lifetime of the opportunity"... So I'm saying yes to this opportunity. It's going to be a lot of work because this is something I'm actually going to HAVE to invest a lot of time towards, and there are things that I will have to figure out family wise: husband, child, home, family time... I have my husband's support, and it's a matter of determination, am I really going to do this? You damn right I am!					

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/840725118322110464)



###  Day 40: Thursday March 9, 2017
#####

**Today's Progress**: some freeCodeCamp JS exercises but couldn't figure out "Profile Lookup"

**Thoughts**: TIREDDDD							

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/840070095409823744)



###  Day 39: Wednesday March 8, 2017
#####

**Today's Progress**: I skipped yesterday because I went to a Women Who Code Hacknight but we didn't code. I ended up talking to two women most of the night. Towards the end I approached a developer who had asked for help on how to get congress people phone numbers based on the user's location, she said there were these other two websites that were getting this information from somehwere but she couldn't figure out their source. So when I approached her - because I was curious and feeling brave - she showed me what she had been able to find that the websites were getting information from a source that had to be hosted "somewhere", she opened her dev tools and showed me the JSON response. She also went over to the Network tab and something else to show the activity of the files (God I know I sound like I don't know what I'm talking about because I don't)... To make a very long story short, I tried to help out with ideas as to how to obtain the info, and then I was inspired to figure out how the troubleshooting worked.

* I will read about markdown something because i need a new paragraph.

* So we went over Troubleshooting JS during my course at GA, and the first part of finding errors in the console is easy. The tricky part was adding debugger and break points, that part kind of went over my head. I went back to the slides and was not able to get anywhere. The only good thing was that I installed JS linter and bracket highlighter for sublime text on this computer.

* I know I'm treating this like a diary and it's so embarrassing hahahaha

**Thoughts**: TIREDDDD							

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/839679248138977280)

2. [Modified file for logic errors](https://github.com/catespinosa/catespinosa.github.io/commit/ed3ca1bf2936acf46980ff689e57b99e0f651f30#diff-52288dd517934f9d38cdf74a9828cf42)


###  Day 38: Monday March 6, 2017
#####

**Today's Progress**: Free Code Camp objects. Started on for loops. Useful reviews especially for accessing [nested objects](https://www.freecodecamp.com/challenges/accessing-nested-objects#?solution=%0A%2F%2F%20Setup%0Avar%20myStorage%20%3D%20%7B%0A%20%20%22car%22%3A%20%7B%0A%20%20%20%20%22inside%22%3A%20%7B%0A%20%20%20%20%20%20%22glove%20box%22%3A%20%22maps%22%2C%0A%20%20%20%20%20%20%22passenger%20seat%22%3A%20%22crumbs%22%0A%20%20%20%20%20%7D%2C%0A%20%20%20%20%22outside%22%3A%20%7B%0A%20%20%20%20%20%20%22trunk%22%3A%20%22jack%22%0A%20%20%20%20%7D%0A%20%20%7D%0A%7D%3B%0A%0A%2F%2F%20Only%20change%20code%20below%20this%20line%0A%0Avar%20gloveBoxContents%20%3D%20myStorage.car.inside%5B%22glove%20box%22%5D%3B%20%2F%2F%20Change%20this%20line%0A%0A) and [nested arrays](https://www.freecodecamp.com/challenges/accessing-nested-arrays#?solution=%0A%2F%2F%20Setup%0Avar%20myPlants%20%3D%20%5B%0A%20%20%7B%20%0A%20%20%20%20type%3A%20%22flowers%22%2C%0A%20%20%20%20list%3A%20%5B%0A%20%20%20%20%20%20%22rose%22%2C%0A%20%20%20%20%20%20%22tulip%22%2C%0A%20%20%20%20%20%20%22dandelion%22%0A%20%20%20%20%5D%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20type%3A%20%22trees%22%2C%0A%20%20%20%20list%3A%20%5B%0A%20%20%20%20%20%20%22fir%22%2C%0A%20%20%20%20%20%20%22pine%22%2C%0A%20%20%20%20%20%20%22birch%22%0A%20%20%20%20%5D%0A%20%20%7D%20%20%0A%5D%3B%0A%0A%2F%2F%20Only%20change%20code%20below%20this%20line%0A%0Avar%20secondTree%20%3D%20myPlants%5B1%5D.list%5B1%5D%3B%20%2F%2F%20Change%20this%20line%0A%0A)

**Thoughts**: Feeling really tired and I've been really busy with work and home... 							

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/838963187668123650)


###  Day 37: Sunday March 5, 2017
#####

**Today's Progress**: Free Code Camp exercises today. Some switch statements, counting cards exercise.

**Thoughts**: Went to the American Museum of Natural History to see the "Cuba!" exhibit and got some inspiration for my site. I wanted to get away from the blue, red and white colors of the Cuban flag, so I saw some nice color combos and use of graphics.							

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/838566742838370304)


###  Day 36: Saturday March 4, 2017
#####

**Today's Progress**: added fullscreen modal for "about" page and more CSS. Added a background image to the rueda call random generator. I'm working backwards, you're supposed to start with the UI and then move on to code but I'm still playing around with the UI.

**Thoughts**:							

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/838232228555599876)


###  Day 35: Friday March 3, 2017
#####

**Today's Progress**: I'm almost done with the Cuban dance site, it's a mashup of things that I learned in the JavaScript course and that I wanted to put into practice before I forgot. It also helped me practice my googling skills especially with the CORS problem I was having. It looks like something but the critic in my thinks it's pointless. It's pulling info from 2 APIs (spotify and meetup) so that's something. I'm using Bootstrap for HTML layout and I used some fancy CSS that I found for hovering over the thumbnails for the spotify tracks. Mobile version still needs some work.

**Thoughts**: I think I'm going to take a break from it and do some tutorials next. Might still do the About page so it looks complete and people know what they're looking at, but after that I think I need to do some learning. I'll continue with FCC challenges.								

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/837903645551263744)


###  Day 34: Thursday March 2, 2017
#####

**Today's Progress**: I copied and pasted code using JSONP for my API call, and switched some stuff around and now I have results on the page. It doesn't quite do what I need it to do yet because I still need to learn more. I want to find meetups based on the user's location, but there are no long or lat coords in the API call so I don't know how I would go about that. The geo location function makes you think that you are searching for groups in your area, but in reality it's fetching data based on my zip code.

**Thoughts**: I might switch to learning next week, I feel like I've wasted time trying to work with proxy server and not knowing how to impement it.									

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/837530252117041158)


###  Day 33: Wednesday March 1, 2017
#####

**Today's Progress**: Not a lot of progress today either. Looked at some php proxy scripts but not sure what to do now.

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/837159244059279360)


###  Day 32: Monday Feb. 27, 2017
#####

**Today's Progress**: Not a lot of progress just looking into proxy servers and how to incorporate one into my project

**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/836434868762468352)

###  Day 30 and 31: Saturday Feb. 25 and Sunday Feb. 26, 2017
#####

**Today's Progress**: Between Saturday and Sunday I have been busy reading more about CORS and watching Youtube videos so that I can find out where to add the headers for my cross origin request. I reached out to an expert web dev in hopes that he could help me figure out what headers to add and where so that i could get away from the error: No 'Access-Control-Allow-Origin' header is present on the requested resource. However, I continued to read and going back to the meetup API docs, and I found that I can only make a CORS request if I'm using OAuth. I don't want to make the user sign on every time they visit the site (are people really going to visit the site?), so what to do now?

** **the blog post I read earlier this week didn't mention any issue with cross origin requests, so I thought it would work. There has to be a way around this. I know there is a way to create a proxy and I think it involves a creating a php file that has your API key so that it's not exposed(?)... all hear say LOL I have to continue to read about this. OMFG. For the record, this is like the second week that I read about this and as hard as it seems, I feel like I'm slowwwwly making progress in understanding this. Just wondering if it's worth it.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/836066788827873281)



###  Day 30 and 31: Saturday Feb. 25 and Sunday Feb. 26, 2017
#####

**Today's Progress**: Between Saturday and Sunday I have been busy reading more about CORS and watching Youtube videos so that I can find out where to add the headers for my cross origin request. I reached out to an expert web dev in hopes that he could help me figure out what headers to add and where so that i could get away from the error: No 'Access-Control-Allow-Origin' header is present on the requested resource. However, I continued to read and going back to the meetup API docs, and I found that I can only make a CORS request if I'm using OAuth. I don't want to make the user sign on every time they visit the site (are people really going to visit the site?), so what to do now?

** **the blog post I read earlier this week didn't mention any issue with cross origin requests, so I thought it would work. There has to be a way around this. I know there is a way to create a proxy and I think it involves a creating a php file that has your API key so that it's not exposed(?)... all hear say LOL I have to continue to read about this. OMFG. For the record, this is like the second week that I read about this and as hard as it seems, I feel like I'm slowwwwly making progress in understanding this. Just wondering if it's worth it.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/836066788827873281)




###  Day 29: Friday, February 24, 2017
#####

**Today's Progress**: Fixed syntax error with my jQuery button - missing # for the button div. I'm able to get a location when I click on it. HOWEVER... I'm getting cross origin requests issues, but I'm not really understanding where you have to put the "headers" or what they are. I'm going to watch a video tomorrow because this is BS. I installed a local server with npm but that still didn't work. I read that I may need to change the URL in my hosts file, but I don't know what I would change it to. Would I add the localhost URL? More tomorrow.

**Pseudo code**:
* Click button to get user's location
* Search nearby groups based on coords.
* Parse API response for: city, name of group, URL, number of members, photo.
* Put results on DOM (create or append to divs)


**Thoughts**: small win today with the location button.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/835310396621869056)


###  Day 28: Thursday, February 23, 2017
#####

**Today's Progress**: Read up on a previous exercise with oAuth to get an idea of what to do with the meetup API since we used the browser's navigator to request geolocation, and I want to search for groups based on the user's location. On the exercise, the js file would ask for the user's location on page load but I want to ask for it when the user clicks a button because I have other stuff on the page. But the on click function did not do anything and I coudln't figure out why, even console.log was not returning anything.



**Thoughts**: I felt intimidated by what I was trying to accomplish and almost did not start working on it because it was going to be too "hard" and it might still be but I have a better understanding now about what i want to do than what i had before.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/834986517600751616)


###  Day 27: Wednesday, February 22, 2017
#####

**Today's Progress**:Crafted my API call using the meetup API console. I found the "Topics" category in order to search for groups in the GET find groups method. I had to find the ID for each topic so that I could pass it as a parameter to my URL. This allowed me to better target the type of music and dance I was looking for (cuban) because by using the "Category ID" I was getting all the dance types. At first I thought I was going to be able to use the find topic method but that only retrieved the info about the topic and I want to be able to display different groups based on location. The results are showing a New York location based on my profile, so I will have to use the browser's geolocation to be able to target the user's location. I will have to review a previous exercise and pray to God (and the old gods and the new) that I can apply it to this exercise.


* (I started writing the below before I found my solution) continued reading about the meetup.com API. I learned a few things that will be challenging and that I'm going to type below to see if I understand them:

* I need to obtain and API key - I've worked with this before but it was in my intro to JS class and I was mainly scared and frustrated. But it's kind of making sense now.  So how do I get an API key? Well, I have to be signed in to the app. I tested one of the sample public callbacks - or endpoints? - and it didn't work because I wasn't logged in, so voila! there's my answer.

* You can avoid exposing your API keys when you do an API call by using an [API Key signature](https://www.meetup.com/meetup_api/auth/#keysign) for meetup which allows you to use the same API call on any app as long as you don't change the parameters or use it for another API method. [Read this for more info](https://www.raymondcamden.com/2015/11/20/using-the-meetup-api-in-client-side-applications)

* API method is how the requests are defined.



**Thoughts**:  I think I spent 2 hours reading this plus 1 hour at work today -_- Crossing fingers. I seriously need to read on markdown 0:-)


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/834602535965044737)



### Day 26: Tuesday, February 21, 2017
#####

**Today's Progress**: added a container class to the random generator section and fixed the video embed. I still need to figure out how to make the page scroll all the way to that section and for the window to scroll down a bit when the video opens. When there is no video the window jumps a bit too. Read about the Meetup API to see how I can incorporate class or meetup information for a specific city.


**Thoughts**: The API might require authorization, but I"m not sure yet. I don't want to keep refreshing a token because I don't feel comfortable with it yet. Lots of information and very little understanding.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/834239456697806849)

### Day 25: Monday, February 20, 2017
#####

**Today's Progress**: A lot of CSS and not a lot of JavaScript today on my cuban dance project. I was able to fix the width of the header since I had the div container tag before the div row tag and I needed the background color of the header to take up the entire width of the page. I got my top nav linking to the anchor ids on the page and need to add a scroll. The random generator button was taking me back to the top on click, so I just had to add an preventDefault method to it and that took care of the problem. Tomorrow I have to fix the width of the videos, they're too big for the page and you can't see them.


**Thoughts**: Good progress today, I just don't know if I can show this to anyone lol I'm scurrrred!


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/833903969026052100)


### Day 24: Sunday, February 19, 2017
#####

**Today's Progress**: Spent a couple of hours figuring out how to hide/show content. I was debating whether to show hidden content within my HTML or to load an external HTML. When I finally figured out how to load HTML, I got the error: XMLHttpRequest cannot load file. Cross origin requests are only supported for HTTP. But before I went too deep into how to fix it, I decided to go with the easier CSS path which would hide the playlists block and show the random generator div -- $('#playLists').hide(); -- simple enough. THis just made me remember that I need to read up on markdown but I'm too lazy right now.  Ok back to my work, once that was working, I went out and then had an "aha!" moment, why was I trying to hide the content and why not make it into a simple single page site? So that's what I'm trying to do now. Read up on Bootstrap tabs but that would have required to change my whole nav and work on the look of it again. Anyway, I've decided what to do already which gives me hope.


**Thoughts**: Since I spent so much time trying to figure a "simple" jQuery problem trying to load the html file into my index.html file, I questioned my approach to this challenge. Should I be learning more at this time? Because I'm copying solutions from stack overflow and when they don't work, I obviously become frustrated. Last week's meetup at WWCNYC inspired me to work on personal projects, but then I go back to feeling like I don't know enough -- yes I know you never know enough -- and should go back to studying so that I can figure out what's wrong with my project. Ok I've talked myself out of this by remembering that it's all a process and maybe this week I'll give the personal project a try. Next week might go back to learning, we'll see.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/833528721600630785)



### Day 23: Saturday, February 18, 2017
#####

**Today's Progress**: I changed the CSS a bit more on the final project, and I read about loading content on the same page with [jQuery](http://www.jqueryscript.net/other/Dynamically-Load-Content-Into-A-Container-with-jQuery.html) but I didn't get it to work.

**Thoughts**: My goals for the 100 days of code challenge were to finish the outstanding project from my JS project, learn angular and es6, create a single page website and my portfolio. But I think I'm going to have to revise those goals or give them a further deadline. I've been inspired to expand on my final project so that's what i'm gonna do for now. I have to focus on one thing so I dont' feel like I'm all over the place (but that's obvious haha)


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/833145359186669568)


### Day 22: Friday, February 17, 2017
#####

**Today's Progress**: After yesterday's meetup I was inspired to continue working on my JS final project. So today I worked on the CSS to make it look more like the spotify UI, when you hover the images you see an overlay of the play button and the opacity of the photo changes. I found [this resource](https://miketricking.github.io/dist/) for making image hover effects in bootstrap but but it doesn't work on my iPhone.

**Thoughts**: Talking with other people about coding inspired me to work on my own projects. I wanted to focus on Free Code Camp exercises this week but I want to get something going on my own.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/832795157862834176)

2. [Cuban music project](https://github.com/catespinosa/catespinosa.github.io/commit/3169c194f77ae0b1d51b8f30a662dbd431573700)


### Day 21: Thursday, February 16, 2017
#####

**Today's Progress**: Attended Women Who code meetup on Algorithms. Worked with the JavaScript group and we solved the Tribonacci and Roman numerals. The tribonacci problem is a sequence that takes the sum of the previous 3 numbers to generate the next number. Tribonacci takes a "signature" or starting array of numbers. Different signatures will generate different sequences. Write a function that takes as it's argument a signature and an "N" and return the first n elements (including the signature). I learned that you can call a variable "let" instead of "var". Also worked on the Roman Numerals problem:  converts an integer to its Roman numeral equivalent. 

**Thoughts**: This was a really good meetup. The girls that I worked with were really open to answering questions and explaining how things worked. Really helpful. I also went with a new friend which I'm happy about.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/832416658341896193)

2. [Tribonacci](https://repl.it/Fmxj/0)

3. [Roman numerals](https://repl.it/FnAu/0)

### Day 20: Wednesday, February 15, 2017
#####

**Today's Progress**: Working on adding the json objects to the dom, also did a free code camp exercise: "Adding a default option in Switch statements"

**Thoughts**: When coding don't go on twitter and read about what you REALLY should be learning or working with.


**Link to work:** 


1. [Today's tweet](https://twitter.com/catespinosa/status/832065881484169220)


### Day 19: Tuesday, February 14, 2017
#####

**Today's Progress**: I was able to resolve the access control issues on the dropbox url. I had to change the URL www.dropbox.com to dl.dropboxusercontent.com and use getJSON method. However, I don't know why that happened, I will read up on it because all of the Access Control documents I read said you had to create functions, and I didn't really understand them -_-  I'm hoping I can figure out how to update the HTML file using the JSON file tomorrow. This will help me with an interim solution to a problem I have at work.

**Thoughts**: I could not get out of bed early enough this morning and I had to go into the office, so I'm coding at night again. I will get up tomorrow but I still need to figure out my morning routine.   


**Link to work:** 

1. [JS file in my repo](https://github.com/catespinosa/catespinosa.github.io/blob/master/updating_html_json/js/app.js)

2. [Today's tweet](https://twitter.com/catespinosa/status/831699074093084674)

### Day 18: Monday, February 13, 2017
#####

**Today's Progress**: Free Code Camp logical operators, if/else, finished golf challenge (lots of if/else statements).

**Thoughts**: So I was wrong about switching https to http, and my app for updating the html file still doesn't work. But it's a new week and I've decided that I will wake up early to code instead of doing it at night because I've been too tired and nights. Since I'm not a morning person, I think working on guided exercises will help with adjusting to coding in the mornings.   


**Link to work:** 

1. [Golf code](https://www.freecodecamp.com/challenges/golf-code#?solution=%0Afunction%20golfScore(par%2C%20strokes)%20%7B%0A%20%20%2F%2F%20Only%20change%20code%20below%20this%20line%0A%20%20if%20(par%20%3C%3D%204%20%26%26%20strokes%20%3D%3D%201)%20%7B%0A%20%20%20%20return%20%22Hole-in-one!%22%3B%0A%20%20%7D%20else%20if%20(par%20%3E%3D%204%20%26%26%20strokes%20%3C%3D%20par%20-%202)%20%7B%0A%20%20%20%20return%20%22Eagle%22%3B%0A%20%20%7D%20else%20if%20(par%20%3D%3D%204%20%26%26%20strokes%20%3D%3D%20par%20-%201)%20%7B%0A%20%20%20%20return%20%22Birdie%22%3B%0A%20%20%7D%20else%20if%20(par%20%3E%3D%204%20%26%26%20strokes%20%3D%3D%20par)%20%7B%0A%20%20%20%20return%20%22Par%22%3B%0A%20%20%7D%20else%20if%20(par%20%3D%3D%204%20%26%26%20strokes%20%3D%3D%20par%20%2B%201)%20%7B%0A%20%20%20%20return%20%22Bogey%22%3B%0A%20%20%7D%20else%20if%20(par%20%3D%3D%204%20%26%26%20strokes%20%3D%3D%20par%20%2B%202)%20%7B%0A%20%20%20%20return%20%22Double%20Bogey%22%3B%0A%20%20%7D%20else%20if%20(par%20%3E%3D%204%20%26%26%20strokes%20%3E%3D%20par%20%2B%203)%20%7B%0A%20%20%20%20return%20%22Go%20Home!%22%3B%0A%20%20%7D%0A%20%20%0A%20%20return%20%22Change%20Me%22%3B%0A%20%20%2F%2F%20Only%20change%20code%20above%20this%20line%0A%7D%0A%0A%2F%2F%20Change%20these%20values%20to%20test%0AgolfScore(5%2C%209)%3B%0A)

2. [Today's tweet](https://twitter.com/catespinosa/status/831111843389272064)


### Day 17: Sunday, February 12, 2017
#####

**Today's Progress**: Uploaded my JSON file to dropbox and installed "Allow-Control-Allow-Origin" extension on chrome to test it.  

**I was getting this error testfile.html:1 XMLHttpRequest cannot load https://www.dropbox.com/s/kmqf99al4l7ntie/stories.json?dl=0. No 'Access-Control-Allow-Origin' header is present on the requested resource. Origin 'null' is therefore not allowed access. 

**So I might just have solved it by removing the s from https, after hours of reading about how to fix this error.

**Read about using  a Google Spreadsheet as your JSON backend, and created one in drive but the response was too weird and I decided to try to continue with the file I had created.

**Thoughts:** -_- feeling very confused and frustrated


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/830890097792917504)


### Day 16: Saturday, February 11, 2017
#####

**Today's Progress**: Pseudo code for how to update an html file with new data and started on the code to parse the data. Hopefully I can use this for a work project I worked on yesterday. 

**Created a JSON file to test updating an index file dynamically. This looks like it might be the long way around but I'm using the example functions from the Feedr app, so hopefully this helps me have a breakthrough with that project. I'm using an html test file to see if my "creation" will work. Found out that I need to install a local web server on my machine in order to run (?) my JSON file(?).

**I got this error XMLHttpRequest cannot load file://stories.json/. Cross origin requests are only supported for protocol schemes: http, data, chrome, chrome-extension, https, chrome-extension-resource.

** Read about how to create JSON from csv and that you can use an online converter. When I converted my csv file, the JSON didn't return the properties correctly, maybe because there were special characters? I hope this doesn't sound stupid because I don't know how to explain it exactly or if I'm using the right terminology.

** Found out what linting means in programming. When you convert csv to JSON it's recommended to validate it with JSONlint, which I didn't do.

**Thoughts:** Again, this might be the difficult way to go about updating the html page.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/830632326812024832)


### Day 14: Thursday, February 9, 2017
#####

**Today's Progress**: Struggled with the Free code camp "stand in line" challenge because of the arguments. Passing arguments is something I still struggle with but I think I'm getting it now. Moved on to boolean, you don't need to declare else in and "if/else" statement? whaaa?

**Thoughts:** NEED TO PRIORITIZE CODING IN THE MORNING - -_-   I can't continue like this, I'm a night owl but I also have a husband and a kid and can't do this anymore.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/829905827305766916)

2. [Stand in line challenge](https://www.freecodecamp.com/challenges/stand-in-line#?solution=%0Afunction%20nextInLine(arr%2C%20item)%20%7B%0A%20%20%2F%2F%20Your%20code%20here%0A%20%20arr.push(item)%3B%0A%20%20%0A%20%20return%20arr.shift(item)%3B%20%20%2F%2F%20Change%20this%20line%0A%7D%0A%0A%2F%2F%20Test%20Setup%0Avar%20testArr%20%3D%20%5B1%2C2%2C3%2C4%2C5%5D%3B%0A%0A%2F%2F%20Display%20Code%0Aconsole.log(%22Before%3A%20%22%20%2B%20JSON.stringify(testArr))%3B%0Aconsole.log(nextInLine(testArr%2C%208))%3B%20%2F%2F%20Modify%20this%20line%20to%20test%0Aconsole.log(%22After%3A%20%22%20%2B%20JSON.stringify(testArr))%3B%0A)


### Day 13: Wednesday, February 8, 2017
#####

**Today's Progress**: JavaScript track on Free Code Camp: manipulating arrays, functions, scope. Took a break to join the #CodeNewbie chat on Twitter.

**Thoughts:** Skipped Tuesday becuase I've been pushing myself too hard while being sick, and I'm glad I did because I'm feeling better today. These challenges will help me with Feedr but I'm not ready to open up that can of worms yet. sigh.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/829538726946684928)


### Day 12: Monday, February 6, 2017
#####

**Today's Progress**: Completed the jQuery challenges on Free Code Camp


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/828817492357369856)





### Day 11: Sunday, February 5, 2017
#####

**Today's Progress**: Made some progress but I'm still really stuck on the feedr app. I was able to show the title for each story in the popup with the only issue being that the h3 is being added to the h1 inside the popup. I can't remember how I set it up (with help of course) I should move on.


**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/828476716905529344)




### Day 10: Saturday, February 4, 2017
#####

**Today's Progress**: Went to a Women Who Code meetup and we were introduced to Xcode and Swift. Created a stickers pack app and a stickers app for iMessage. The first one was easy to set up, the second one allowed for more customization because you could manipulate the code. We used a for loop to iterate through my stickers so they could be diplayed.


**Link to work:** 

1.	[iOS Sticker app](https://github.com/catespinosa/iOS-stickers.git)


2. [Today's tweet](https://twitter.com/catespinosa/status/827965924569444354)



### Day 9: Friday, February 3, 2017 (into Saturday)
#####

**Today's Progress**: Looked into Feedr again and read about "this" and closures because it looks like it's got something to do with it LOL Not sure how to move forward. When I click on the headline only the first popup opens, so the issue is not with the link but with the function opening the popup. I've stared at the code for a long time and did some guessing which I know is not good. 

**Thoughts:** I found the solution in another repo but they use a different approach and I am far along with mine so I will have to decide what to do. Hopefully some sleep and luck will help tomorrow... I need to code during the day, seriously!!


**Link to work:** 

1.	[Feedr](https://github.com/catespinosa/catespinosa.github.io/tree/master/jsd920_class_repo/projects/feedr)


2. [Today's tweet](https://twitter.com/catespinosa/status/827759295047557120)





### Day 8: Thursday, February 2, 2017
#####

**Today's Progress**: Reviewed basic Javascript concepts at FreeCodeCamp. Solved "convert celsius to fahrenheit" and "word blanks" exercises. I created two repos for 2 of my projects which counts as coding in my book since I'm still getting used to git.


**Thoughts:** I will continue with the freecodecamp js exercises tomorrow so I can dedicate a little more time to the Feedr app during the weekend and hopefully find a solution to getting the first story every time I click on any headline.

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/827364555462365185)


### Day 7: Wednesday, February 1, 2017 (dont know)
#####

**Today's Progress**: Not much progress today. I'm still getting the first story when I click on any link but didn't really know how to approach it and I can't explain it to google. Signed up with Free Code Camp.


**Thoughts:** Trying to code every day is hard. I'm tired and frustrated because I can't get it to work.

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/827003923760295941)



### Day 6: Tuesday, January 31, 2017 (2:15 hrs)
#####

**Today's Progress**: Working on the Feedr project. The #popup .loader class was not going away because I was trying to use $('#popUp').removeClass('.loader hidden'); without realizing that the period before loader needed to be removed, so when I previewed the app only "hidden" would be removed... I spent almost 2 hours wondering how the "loader" class was being added to "#popup" GRRRRR!!!!! But alas, I figured it out!!! It was so simple -_-  . 

I was able to show the content inside the popup by creating a function to add more content to the handlebars template and also found out I had to move the script tag to encompass all the content I wanted inside the template. I had to move the firs template down inside the HTML (maybe i could have moved the popup html code up but this worked). Need to figure out how to display the text for the story that I click on since it's only showing the first story no matter what link I click on.

I moved on to the close button but couldn't get it to work.


**Thoughts:** I need to code earlier. I'm tired but wired up from coding.

**Link to work:** 
1. [Feedr project](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/feedr/js/app.js)

2. [Today's tweet](https://twitter.com/catespinosa/status/826639675733458946)




### Day 5: Monday, January 30, 2017 (1 hour)
#####

**Today's Progress**: Very little: Continued to work on the GA Feedr project that I had started during my JSD course, I was able to write one line of code that worked to show the modal when you click the headline, but can't figure out how to show the content inside it.

**Thoughts:** I think I'm not targeting the div properly. I tried using css and empty quotes to remove "display: none" but that didn't work. Also "removeAttr"... More tomorrow... JUST REALIZED I DIDN'T READ MY OWN PSEUDO CODE!! tired and going to bed.

**Link to work:** 
1. [Feedr project](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/feedr/js/app.js)

2. [Today's tweet](https://twitter.com/catespinosa/status/826260816290783232)




### Day 4: Sunday, January 29, 2017 (2.5 hours)
#####

**Today's Progress**: Made the videos on my rueda generator responsive and continued to play around with the style of the page. Completed 2 HTML 5 exercises in General Assembly's Dash.

**Thoughts:** Felt like I've spent way too much time on the random call generator but I learned some things and felt confident with the code. I decided to move on to exercises in General Assembly's Dash and learned some HTML 5 and CSS tricks that I didn't know about. I need to read about Markdown so I can style my readme file properly.

**Link to work:** 
1. [Rueda call generator](https://catespinosa.github.io/jsd920_class_repo/projects/final_project/public/rueda-random-gen.html)
2. [Today's tweet](https://twitter.com/catespinosa/status/825916606538711040)



## Day 3: Saturday, January 28, 2017

**Today's Progress**: Continued working on my random rueda call generator using JQuery.

*Added an iframe hide on page load and show on click.

*Added if/else statement to display the iframe only when there is a video url

*Still learning to work with Bootstrap. Need to improve the layout.

*Added new classes to css file


**Thoughts** 

*[Worked with this list of turn patterns and the videos they provide](https://en.wikibooks.org/wiki/Rueda_de_Casino/Moves_for_Beginners)
Since some of the moves on this list don't have a video associated with it, an empty iframe would still show up when I clicked the button. I read about how to access properties on objects and I figured I had to add an if/else statement after clicking the button to check whether the key value, in this case the youtube URL, exists. I don't know what the correct way is but I wanted all my objects to have the same number of properties so I opted for leaving the videosource property in each object and when I didn't have a video URL I added empty quotes. My if/else statement checks for the empty quotes key value and if true then it doesn't display the iframe in the DOM.

*I read about the object method "hasOwnProperty" for checking whether an object has the property you are looking for. I could have used this if I had removed the property "videosource" from the objects that didn't have a video. [Determining if an object property exists](https://www.nczonline.net/blog/2010/07/27/determining-if-an-object-property-exists/) 

**Errors** Found this error when trying to display the youtube video for the specific turn pattern: Refused to display 'https://www.youtube.com/watch?v=Y0U309VrG2w&feature=youtu.be' in a frame because it set 'X-Frame-Options' to 'SAMEORIGIN'. Then I found this solution on stackoverflow: 
If you are getting this error for a YouTube video, rather than using the full url use the embed url from the share options. It will look like http://www.youtube.com/embed/eCfDxZxTBW4. So I had to go back and copy the Embed URLs for the videos. It's fine since I'm keeping my list of turn patterns small. [Link to answer](http://stackoverflow.com/questions/6666423/overcoming-display-forbidden-by-x-frame-options)


**Link(s) to work**
1. [Rueda de Casino random rueda call generator](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/final_project/public/rueda-random-gen.html)
2. [Today's tweet](https://twitter.com/catespinosa/status/825446248626974723)


### Day 2: Friday, January 27, 2017
#####

**Today's Progress**: Added video source object to my random rueda call generator and it worked. Need to find out how to hide the iframe on page load. I'm using the same video for testing purposes but I need to find videos for all the rueda calls.

**Thoughts**: I didn't spend a full hour today and I feel guilty since it's day 2! I have to attend a function but I'm hoping to get a little more coding in today. It was a stressful day for a Friday.

**Link(s) to work**: 

1. [Rueda de Casino random rueda call generator](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/final_project/public/rueda-random-gen.html)

2. [Today's tweet](https://twitter.com/catespinosa/status/825161201286074368)


### Day 1: Thursday, January 26, 2017
#####

**Today's Progress**: Cloned my own repo, 100Days repo and Javascript30 to my new computer. Config'd my user name and email address in git because all the work that I had done during my JS course was not showing up in my contribution chart.

**Thoughts:** READ and FOCUS! You got this!

#### Useful links: 

*[Why are my contributions not showing on my profile](https://help.github.com/articles/why-are-my-contributions-not-showing-up-on-my-profile/)

*[How to show or change your Git username or email address](http://alvinalexander.com/git/git-show-change-username-email-address)

**Link to work:** [Contribution chart shows one commit today :)](https://github.com/catespinosa)

* [Today's tweet](https://twitter.com/catespinosa/status/824843788145168384)









