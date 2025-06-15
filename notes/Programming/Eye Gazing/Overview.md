![[Pasted image 20250602165515.png]]
# Process
1. Acquire video frames
2. Image pre-processing
3. Face detection
4. Eye patch extraction
5. Finding COI / Pupils
6. Eye Corner Extraction
7. Point of Gaze calcualtion


It proposes to use the Y CbCr color space for face detection, which is considered
to be one of the best approaches in color images.

![[Pasted image 20250602170216.png]]

**Note: tint-saturation-luma (TSL) color space provides best results

** Drawback: This technique was applied to several images of different resolutions and various head postures with different lighting conditions. The drawback in face detection was it detected only Asian faces with wheatish complexion. After observing results, the rate of false detections was more severe in case of eyes detection

=> Conclusion: skip these processes and instead force user to put face into bounding box for eye patch extraction

** Note: “Sobel” edge detector is being used in this algorithm, because it resulted in more accurate detections

Firstly, algorithm was applied on images acquired by a low resolution webcam i.e. 640X480(VGA) and pupil detection accuracy didn’t prove satisfactory. As an interesting investigation, algorithm was applied on frames acquired by high resolution webcam i.e. 1280x720(HD 720p) and it resulted in far better detection accuracy, the results were quite accurate, but the processing time per frame was more than expected i.e. 600–700mS. As this project is supposed to be a real-time project, which requires a less computational cost, and it needs to work at least at a frame rate of 15fps, which means complete processing time for each frame should not be more than 66mS. Therefore, it was decided to move on using OpenCV library for algorithm implementation, as the algorithms developed using OpenCV are light weight and have less computational cost

=> From MATLAB to OpenCV for implementation

# Gaze estimation
Gaze estimation means to learn from usage statistics data and predict the next value of mouse pointer based on probabilities of regions and previous movements of pointer using different algorithms. For the estimation, we started from very basic prediction mechanisms and then gradually developed algorithm using different basic and advanced techniques. These are discussed in gradual steps in different sub-sections of this topic.

** Note: Regression can be a useful tool for prediction, if human eye movements follow some equation model, based on prior observation we came to the conclusion that we cannot describe human eye ball movements by any equation model, as they are more or less random, with still and slower movements as well as faster and larger movements.

=> Conclusion:  After some calculations, it was concluded that regression is not useful for gaze prediction problem and deferred the task to find some relevant filtering or prediction techniques.

# Filter 
Usage of Filters is not new in tracking and estimation applications. Literature review suggested that two of the most common filters could be used in the case of gaze estimation problem i.e. Wiener filter [23] or Particle filter [24].

# OpenCV pre-trained models
OpenCV is called Haar Cascade Classifier and uses simple rectangular features, called Haar features

# Good features to track
All of the above mentioned algorithms were applied for eye corner detection, but only “Template Matching” technique available in OpenCV library to detect eye corners, yielded satisfactory results. This algorithm resulted in satisfactory performance at a fast processing speed. Processing time for each frame using this algorithm was 10–15 mS.

# Point of Gaze Calculation

# Pupil detection Conclusion
While analyzing the results, it was concluding that applying a threshold between previous frame pupil location and present frame pupil location, accuracy can be enhanced. After applying the threshold, the accuracy improved to 87% with a slight increase of 0.5–1mS processing time per frame.


![[Pasted image 20250603105857.png]]