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

**Thoughts:** Felt like I've spent way too much time on the random call generator but I learned some things and felt confident with the code. I decided to move on to exercises in General Assembly's Dash and learned some HTML 5 and CSS tricks that I didn't know about.

**Link to work:** 
1. [https://github.com/catespinosa](https://github.com/catespinosa)
2. [Today's tweet](https://twitter.com/catespinosa/status/825916606538711040)

