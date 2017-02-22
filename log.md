# 100 Days Of Code - Log

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









