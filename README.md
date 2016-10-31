# youtube
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
Simply add autoplay=1 

Value 0 (default): The video will not play automatically when the player loads.

Value 1: The video will play automatically when the player loads.

For example: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/oBu-pQG6sTY?list=PLZ9P66e5V_5VJstoGk8WAaO8NPhYZzVjn?autoplay=1" frameborder="0" allowfullscreen></iframe>

##For a playlist use a comma to separate each video.