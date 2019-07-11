## Bessel’s Correction: Why Use N-1 For Variance/Standard Deviation?
 * because if you use n-1 instead of n, that is sample data of population, it gives accurate result of variance and Standard Deviation.
 * n is the no. of sample data.
 * if you have a sufficiently large sample _and_ if you are actually trying to approximate the population mean.
 * If you’re just interested in finding the sample mean,
 * and don’t want to extrapolate your findings to the population, just omit the correction.
 * When you have an entire population and calculate  the population variance or population standard deviation, results will be accurate. That’s because we have all the data about your population.
 * However, when you work with sample. you’ve only got a small fraction of the population to work with. Therefore, your answers aren’t going to be as accurate as those you would have got, if you had the entire set of data to work with.
The formula for the **sample standard deviation** is similar:  
![](https://www.statisticshowto.datasciencecentral.com/wp-content/uploads/2013/11/sample-standard-deviation.jpg)

In the case of the sample variance & standard deviation, the particular statistic you are working with is the sample mean (x̄) instead of the  population mean (μ). Any x-value in your sample is going to be closer to x̄ than to μ.

The sum of squares for μ  
![](https://www.statisticshowto.datasciencecentral.com/wp-content/uploads/2018/07/ss1.png)

is going to be larger than the sum of squares for x̄.  
![](https://www.statisticshowto.datasciencecentral.com/wp-content/uploads/2018/07/ss0.png)
