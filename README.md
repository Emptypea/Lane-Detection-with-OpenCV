# Lane-Detection-with-OpenCV
Lane are detected in the video using image processing techniques available in the OpenCV library

This project is the implementation of Lane Detection Algorithm used in [https://www.geeksforgeeks.org/opencv-real-time-road-lane-detection/](url)
The working of the code has been demonstrated step by step using a single image. The algorithm is able to detect lines on the road by applying the following steps:
1. The image is preprocessed to remove noise by applying Gaussian Blur with a kernel size 5
2. Edges are detected using Canny Edge detector with min_threhold = 100 and max_threshold = 200
3. We separate the region of interest using mask and manually choosing 4 points that best suit the application.
4. We find the points along the detected lines by using Probabilistic Hough Transform. Then we find the average of all the lines detected to get left and right lanes
5. We draw the lines onto the frames to get the final output.
