# Discussion

I decided to use Gaussian (linear) and Median (non-linear) filters to compare linear vs non-linear methods for image denoising. After experimenting with the tradeoffs higher and lower values gave, I assigned the sigma a value of 0.5. This offered the best balance because a higher value was associated with blurrier images and a lower value with a higher variance. The three histogram tables below illustrate the difference between both filters for each noise level among the data sets. Both the Gaussian and Median filters appeared to reduce noise and smooth out variability. The Gaussian filter is generally noisier than the Median filter, and adjusting the sigma value would either make the image blurrier or increase the variance too much. The images below the histograms show that the Gaussian filter appeared to contain more static but had sharper edges. The Median filter appeared to be blurrier but contained less static. Both filters appeared to make all the noisy images easier to see and read overall. 

After comparing the effectiveness of the filters, I used the Sobel edge enhancement technique to further improve the smoothing. Edge enhancement is the next step after filtering to help improve the edges and picture quality as a whole. I applied this enhancement to every instance of the smoothing across all of the datasets. After that, I compared the images between the original noisy ones, the smoothed ones, and the newly enhanced ones. In the next set of photos,  the enhanced have more clarity, especially around the edge of the brain. The enhanced Median-filtered photos appear to have the most noticeable difference after enhancement because of the blurring that was done beforehand. Since the blurring was more prominent among the Median smoothed ones, the enhancement among the edges makes the photo look clearer. Finally, I calculated the Coefficient of Variation (CV) among all of the images. This calculation is measured by dividing the standard deviation by the mean for each image. A lower CV value indicates a better restoration of the noisy image while a higher value indicates more dispersion around the mean. Across all of the data, the enhanced images had the lowest CV when compared to the regular filter and original noisy image. This is consistent with the images themselves as the enhanced images appear clearer and less noisy. The highest variance of the filtered photos was the T1 3 % noise median smoothed while the lowest variance was the PD 9% noise-enhanced Gaussian smoothed images.

Using the images and CV values, the Gaussian and Median filters when enhanced using Sobel edge enhancement were able to denoise the initial noisy images the best across all modalities. 

