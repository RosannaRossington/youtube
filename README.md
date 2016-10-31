# Videos using HTML5

Before HTML5 to play videos you needed to use a browser plugin like flash.
The easiest way to play videos in HTML, is to use YouTube.

YouTube will display an id (like XGSy3_Czz8k), when you save (or play) a video.

You can use this id, and refer to your video in the HTML code.

##To play your video on a web page, do the following:

- Upload the video to YouTube
- Take a note of the video id
- Define an <iframe> element in your web page
- Let the src attribute point to the video URL
- Use the width and height attributes to specify the dimension of the player
- Add any other parameters to the URL (see below)

You can also navigate to the YouTube page, click the Embed tab and copy the syntax.

For example: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/oBu-pQG6sTY?list=PLZ9P66e5V_5VJstoGk8WAaO8NPhYZzVjn" frameborder="0" allowfullscreen></iframe>

##To autoplay the video 
Simply add autoplay=1 at the end of the URL

Value 0 (default): The video will not play automatically when the player loads.

Value 1: The video will play automatically when the player loads.

For example: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/oBu-pQG6sTY?list=PLZ9P66e5V_5VJstoGk8WAaO8NPhYZzVjn?autoplay=1" frameborder="0" allowfullscreen></iframe>

##For a playlist use a comma to separate each video.

##YouTube Loop
- Value 0 (default): The video will play only once.

- Value 1: The video will loop (forever).

##YouTube Controls
- Value 0: Player controls does not display.

- Value 1 (default): Player controls display.

##Making an iFrame responsive
Setting a height is required, otherwise browsers will render the iframe at a static height of 150px1,

Option 1
Wrap the video in another element which has an intrinsic aspect ratio(__Aspect ratio is the relationship of the width of a video image compared to its height. The two most common aspect ratios are 4:3, also known as 1.33:1 or fullscreen, and 16:9, also known as 1.78:1 or widescreen.__(With intrinsic dimensions, a new width triggers a new height calculation, allowing videos to resize and giving them the ability to scale the same way images do.) ), then absolute position the video within that. That gives us fluid width with a reasonable height.

However lots of classes are needed to adjust different videos.