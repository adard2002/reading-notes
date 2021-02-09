# Reading 02 Notes

[Home](README.md)

## pg 293-301 Chapter 7: JQery
### What is JQery?
This is a JavaScript file that lets you find elements using CSS-style selectors and then can do whatever you want with the elements using JQuery methods.
Example: $('li.hot') This selects every li element with the class of hot.
### Why use Jquery?
Instead of having to write out a whole bunch of stuff in your normal JavaScript file JQuery makes it much much simpler to type out and shorter. 
1. Simple selectors
2. common tasks using less code and typing less
3. cross-browser compatibility

## pg 306-331
### Grabbing single elements vs multiple elements
The $('ul') is an example of single element. Because the ul element in html contains several li elements within that one tag. Then the $('li') is an example of multiple elements that are contained within a single element of ul or ol. 
### Making sure a page is ready to work with
$(document).ready(function(){
  // script goes here
});
The document part represents the page whil the ready even method is when whatever code is inside that function is ready it will run.


## pg 354-357
### How to place your scripts
It is important to know where to place your script tags and script code because this will help the web page render quicker. It is important to place it right before the closing body tag in the html file. This is because we want the HTML to all be loaded first and once that is loaded the the site can worry about rendering the JS and Jquery.


## 6 Reasons for pair programming
1. It helps when you have 2 sets of eyes looking at the same code at the same time and this helps with catching simple errors such as spelling and missing semicolons or any other missing things. And it helps just having someone there to help you. They can catch when you have done something wrong and make a simple mistake.


## 332-335 (Javascript and JQery book)
1. Using Jquery you are able to show or hide elements along with making the elements animate by fading it in or out, or sliding them up or down.If there is an element that has a fancy fade or slide in it. The other elements around it may move to help make room for the animation. 
2. This enhances collaboration between two programmers when focusing on the same code. It's more engaging when there is more than one person looking at the same code. Which makes it harder to slack off and get distracted and procrastinate. 
3. It is very simple and easy to learn from other students or teachers when they see you've made a mistake they can correct you right away and steer you in the right direction.
4. This helps improve social skills. Everyone has their own code handwriting or way they write code. It is important to ask questions if you are unsure of what code runs or does what. It is really good to know how to be able to talk to people. And I really need to work on that too since I have social anxiety lol. 
5. This improves job interview readiness. This is because there are a lot of questions to be asked and answered while looking at another's code. It is good to be able to talk and answer a question efficiently while not rambling or stumbling over words.
6. Work environment readiness. This is because people who want to be a programmer when they get older and want to pursue that dream will need to have experience in what may be used throughout the real world and work field for this career area. It is good to know what exactly you are getting yourself into no matter what job. 


## 302-305  (Javascript and JQery book) I do read these I just don't write things down for the skims yet