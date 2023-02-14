This page shows how Apple creates their famous moving backgrounds used on Product pages. \n
Smaller in scale but the core concept comes across. 
Utilizes the <canvas> tag.
The background is not a video but an jpg file.
A set number of frames loads in the exact number of images needed to complete the animation.
JS noting the user's scroll position decides what frame to render.
Now you might think "Hey that sounds like a lot of images to load in" and you'd be correct.
But the images are pre-loaded when the page renders. That way a new request is not fired of for every frame the user scrolls.
I added some extra logic to measure the screen width to switch the canvas aspect ratio and the small vs large file size.
Have fun scrolling!

Working example at: http://chris-chafin.com/canvas/canvas.html
