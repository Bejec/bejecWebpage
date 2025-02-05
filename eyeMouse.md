# EyeMouse Project

This project demonstrates using eye tracking to take control of mouse movement.  
I also explored using multiprocessing and multithreading to enhance performance.
[Github Project Link](https://github.com/Bejec/FocusFinder)

The idea that started the project is that nothing beats pixels per degree (PPD) than a monitor at a distance away from you.  So instead of creating an AR/VR/XR environment, just use any screens as the environment.  This is more for using the eyes as a human input device rather than creating objects in the environment.

Project was ultimately terminated because of my lack of skill with optics and 3D CAD design.  Ideally the camera should have low FOV, high resolution and positioned in front of the eye.  Was going to use a glass panel to reflect eye image to a camera pointing downward.

<div class="video-container-16by9">
  <iframe
    frameborder="0"
    title="YouTube video player"
    allowfullscreen
    width="560"
    height="315"
    src="https://www.youtube.com/embed/dW3LniF6BbY?enablejsapi=1&mute=1"></iframe>
</div>

The video above shows a mapping of where the eye is looking at on the screen.  You do have to keep your head in the same position as the point of this is to enable gaze visualization in the video below.

<div class="video-container-16by9">
  <iframe
    frameborder="0"
    title="YouTube video player"
    allowfullscreen
    width="560"
    height="315"
    src="https://www.youtube.com/embed/jEYcn5cFrLg?enablejsapi=1&mute=1"></iframe>
</div>

The video above is the furthest I got with what I was trying to achieve.  There is a camera on my forehead that is looking forward. Then there are two cameras looking at my eyeballs.  The eye tracking will cut out and move a window in the forward looking video to show what I am seeing.  The video is very jumpy since I favored accuracy and speed over smoothness.

## Project Goals

The main objectives of this project were to explore how much computation is needed to track eye movement
with an accuracy that rivals real eyesight.  A lot of computation is needed for accurate and quick eye tracking.  To get better image either the camera FOV needs to be reduced (zoomed in) or placed closer to the eye.

## Code:
[Github Project Link](https://github.com/Bejec/FocusFinder)


## Extra Video for seeing eye saccades

<div class="video-container-16by9">
  <iframe
    frameborder="0"
    title="YouTube video player"
    allowfullscreen
    width="560"
    height="315"
    src="https://www.youtube.com/embed/VzT1Xz3-9jY?enablejsapi=1&mute=1"></iframe>
</div>

