# 100 Days Of Code - Log

### Day 1: Thursday, January 26, 2017
#####

**Today's Progress**: Cloned my own repo, 100Days repo and Javascript30 to my new computer. Config'd my user name and email address in git because all the work that I had done during my JS course was not showing up in my contribution chart.

**Thoughts:** READ and FOCUS! You got this!

#### Useful links: 

*[Why are my contributions not showing on my profile](https://help.github.com/articles/why-are-my-contributions-not-showing-up-on-my-profile/)

*[How to show or change your Git username or email address](http://alvinalexander.com/git/git-show-change-username-email-address)

**Link to work:** [Contribution chart shows one commit today :)](https://github.com/catespinosa)

* [Today's tweet](https://twitter.com/catespinosa/status/824843788145168384)

### Day 2: Friday, January 27, 2017
#####

**Today's Progress**: Added video source object to my random rueda call generator and it worked. Need to find out how to hide the iframe on page load. I'm using the same video for testing purposes but I need to find videos for all the rueda calls.

**Thoughts**: I didn't spend a full hour today and I feel guilty since it's day 2! I have to attend a function but I'm hoping to get a little more coding in today. It was a stressful day for a Friday.

**Link(s) to work**: 

1. [Rueda de Casino random rueda call generator](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/final_project/public/rueda-random-gen.html)

2. [Today's tweet](https://twitter.com/catespinosa/status/825161201286074368)


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

### Day 4: Sunday, January 29, 2017 (2.5 hours)
#####

**Today's Progress**: Made the videos on my rueda generator responsive and continued to play around with the style of the page. Completed 2 HTML 5 exercises in General Assembly's Dash.

**Thoughts:** Felt like I've spent way too much time on the random call generator but I learned some things and felt confident with the code. I decided to move on to exercises in General Assembly's Dash and learned some HTML 5 and CSS tricks that I didn't know about. I need to read about Markdown so I can style my readme file properly.

**Link to work:** 
1. [Rueda call generator](https://catespinosa.github.io/jsd920_class_repo/projects/final_project/public/rueda-random-gen.html)
2. [Today's tweet](https://twitter.com/catespinosa/status/825916606538711040)

### Day 5: Monday, January 30, 2017 (1 hour)
#####

**Today's Progress**: Very little: Continued to work on the GA Feedr project that I had started during my JSD course, I was able to write one line of code that worked to show the modal when you click the headline, but can't figure out how to show the content inside it.

**Thoughts:** I think I'm not targeting the div properly. I tried using css and empty quotes to remove "display: none" but that didn't work. Also "removeAttr"... More tomorrow... JUST REALIZED I DIDN'T READ MY OWN PSEUDO CODE!! tired and going to bed.

**Link to work:** 
1. [Feedr project](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/feedr/js/app.js)

2. [Today's tweet](https://twitter.com/catespinosa/status/826260816290783232)


### Day 6: Tuesday, January 31, 2017 (2:15 hrs)
#####

**Today's Progress**: Working on the Feedr project. The #popup .loader class was not going away because I was trying to use $('#popUp').removeClass('.loader hidden'); without realizing that the period before loader needed to be removed, so when I previewed the app only "hidden" would be removed... I spent almost 2 hours wondering how the "loader" class was being added to "#popup" GRRRRR!!!!! But alas, I figured it out!!! It was so simple -_-  . 

I was able to show the content inside the popup by creating a function to add more content to the handlebars template and also found out I had to move the script tag to encompass all the content I wanted inside the template. I had to move the firs template down inside the HTML (maybe i could have moved the popup html code up but this worked). Need to figure out how to display the text for the story that I click on since it's only showing the first story no matter what link I click on.

I moved on to the close button but couldn't get it to work.


**Thoughts:** I need to code earlier. I'm tired but wired up from coding.

**Link to work:** 
1. [Feedr project](https://github.com/catespinosa/catespinosa.github.io/blob/master/jsd920_class_repo/projects/feedr/js/app.js)

2. [Today's tweet](https://twitter.com/catespinosa/status/826639675733458946)


### Day 7: Wednesday, February 1, 2017 (dont know)
#####

**Today's Progress**: Not much progress today. I'm still getting the first story when I click on any link but didn't really know how to approach it and I can't explain it to google. Signed up with Free Code Camp.


**Thoughts:** Trying to code every day is hard. I'm tired and frustrated because I can't get it to work.

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/827003923760295941)

### Day 8: Thursday, February 2, 2017
#####

**Today's Progress**: Reviewed basic Javascript concepts at FreeCodeCamp. Solved "convert celsius to fahrenheit" and "word blanks" exercises. I created two repos for 2 of my projects which counts as coding in my book since I'm still getting used to git.


**Thoughts:** I will continue with the freecodecamp js exercises tomorrow so I can dedicate a little more time to the Feedr app during the weekend and hopefully find a solution to getting the first story every time I click on any headline.

**Link to work:** 

1. [Today's tweet](https://twitter.com/catespinosa/status/827364555462365185)

### Day 9: Friday, February 3, 2017 (into Saturday)
#####

**Today's Progress**: Looked into Feedr again and read about "this" and closures because it looks like it's got something to do with it LOL Not sure how to move forward. When I click on the headline only the first popup opens, so the issue is not with the link but with the function opening the popup. I've stared at the code for a long time and did some guessing which I know is not good. 

**Thoughts:** I found the solution in another repo but they use a different approach and I am far along with mine so I will have to decide what to do. Hopefully some sleep and luck will help tomorrow... I need to code during the day, seriously!!


**Link to work:** 

1.	[Feedr](https://github.com/catespinosa/catespinosa.github.io/tree/master/jsd920_class_repo/projects/feedr)


2. [Today's tweet](https://twitter.com/catespinosa/status/827759295047557120)


