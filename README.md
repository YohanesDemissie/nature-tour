# nature-tour
Advanced CSS Flex Box Grid and Animation

#Reset CSS
to remove all default margins and padding 
example: H1 tag has default padding/margin
reset helps start clean and completely customize and control every element and its layout without default setting intervening 

#box-sizing: border-box;
Adds the total space of margin/padding px to the box over all declauerd height, pixel, width, etc

#height: 95vh;
height of view point. so the view point will be 95% of the container/element box

#  background-size: cover;
makes an image fit the size of the container/elemnent box. Because the above view port is set to 95, the image will fit only 95% of the height

#clip-path: polygon(0 0, 100% 0, 100% 200px, 0 100%);
this is how yuo cut an image and customize what shows by selecting the x, y coordinates  by either percentage or pixels as demoed above

#bennettfeely.com/clippy/
for all customizable shape coordinates you can copy and paste in to your CSS file

#check Node version
in terminal run node --eval 'console.log(process.version)' to check which version of node you are using.

#CSS Order of Styling
Always style in order of html element that way it is in .html file and the way it displays in the browser

#Basic Animation
  animation-name: moveInLeft; which comes with options and directions of animation
  animation-duration: 5s; duration of animation

  #Advanced Animation
  @keyframes moveInLeft { this is the animatino name created by me, above
  0% { special directions for animation at 0% time/location duration
      opacity: 0;
      transform: translateX(-100px); /* negative numbers move to the left, postitive to the right jsut like a graph */
  }

  /* 50% { we can set any animation to any percentage

  } */

  100% {
      opacity: 1;
      transform: translate(0);
  }
}

animation-iteration-count: 5;
the above code repeats the animation 5 times

animation-timing-function: ease-in; //eases in the animation that speeds up in end
animation-timing-function: ease-out; //starts animation regular timing then speeds up towareds the end

# ANIMATION SUMMARY
-- you can summarize animnation reules with simply grouping animation styles like so
  animation: moveInRioght 1s ease-out; and CSS will be able to asign the right properties

--hides all flaws of animation and glitchiness
  backspace-visibility: hidden; 

-- take any element/class/ID and put a hover animation like so...
  .logo:hover {
  animation: moveInRight 1s ease-out;
  }

#Pseudo Classes
This is when a  css selector has a specific command for an element like :hover, :checkbox, selecting last child (which I'm not sure how to apply)... examples below

.button:link {
  background-color: white;
}

.button:visited {
  background-color: purple; //changes color when clicked
}

.logo:hover { #### NOT WORKING AS EXPECTED. COME BACK TO IT LATER ######
  animation: moveInRight 1s ease-out;
} 

