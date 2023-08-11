# sparseOpticalFlow

Created before I started using GitHub. 

Sparse optical flow detection using openCV-4.5.1.

If you have openCV installed at "C:\opencv\.." you will need to edit the CMakeLists.txt on line 7.

On line 15 of main.cpp, remove 
  --full_path_to_video--
and replace it with the actual path on your storage device to the video.

If you wish to use a live webcam feed instead of a video, 
comment out line 15 and uncomment line 16.
