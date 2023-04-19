# Fuzzy Color Image Enhancement - Fuzzy Logic Course - ITE 5th Year


**This repo is migrated to: https://github.com/mo-waseem/fuzzy-color-image-enhancements**


- This code is an implementation for a color image enhancement algorithm that mentioned in: 
    https://www.researchgate.net/publication/237202014_Color_Image_Enhancement_Using_the_Support_Fuzzification_in_the_Framework_of_the_Logarithmic_Model
## Abstract
We can enhance the colors in an image by tunning two things brightness and contrast, this algorithm devided the image into fuzzy 
windows and every pixel has a membership degree to every window, the membership degrees are calculated depending on 
the distance between the window and the pixel, then the means and variances are calculated with respect to the membership degrees,
the final image is obtained by summing up the images of every fuzzy window in a weight way, the weights used are membership degrees.
## Algorithm Steps
  1. Convert the image to gray level space (if it is rgb convert every channel and work on one channel at a time then re-merge them).
  2. Calculate the pixels weights for every window.
  3. Calculate windows means and variances in a wieghted way.
  4. Do b_ij*f + a_ij where "a_ij" is the mean of ij window, "b_ij" is the variance of ij window, "f" is the image.
  5. Summing up the images of every fuzzy window in a weighted way.
## Results
- Grayscale:

![alt text](https://github.com/WaseemKn/FuzzyColorImageEnhancement-FuzzyLogicCourse-ITE5thYear/blob/master/Images/einsteineEnhanced.PNG)

- RGB:

![alt text](https://github.com/WaseemKn/FuzzyColorImageEnhancement-FuzzyLogicCourse-ITE5thYear/blob/master/Images/monkeyEnhanced.PNG)
