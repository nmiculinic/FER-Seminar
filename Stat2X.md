[Online interactive book](http://www.stat.berkeley.edu/~stark/SticiGui/index.htm)

#Stat 2X.1
[MOOC](https://www.edx.org/course/introduction-statistics-descriptive-uc-berkeleyx-stat2-1x)

##Week 1
###Variable
* quantitative
	* discrete
	* continuous
* categorical | qualitative
	* color
	* race
* qualitative ordinal
	* temperature - cold, mild, hot

###Bar Graph
![Bar Graphs](http://getwordwall.com/Attachments/Screenshots/Play/bar-graph.png)

###Stem and Leaf plot
![Steam and Leaf Plot](http://www.mathatube.com/images/stem_ans_leaaf_plot-008.jpg)

###Distribution table
In intervals data clustering left endpoint included, right excluded. Outliers concatenated into endpoint buckets.
![Distribution table example](http://www.kwiznet.com/px/homes/i/Math_Contest_Prep/stat_freqtable3.gif)

###Histogram
*Area* of the bar = *percent* in the intervals
![Example Histogram](http://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Cumulative_vs_normal_histogram.svg/2000px-Cumulative_vs_normal_histogram.svg.png)

###Percentiles
p-th percentile is value such that p percent of the data is less or equal then. When assessing percentiles within histograms we assume values are uniformly distributed with a bar.
* 25th percentile = lower quartile
* 50th percentile = median
* 75th percentile = upper quartile

The pth percentile of a list of numbers is the smallest number that is at
least as large as p% of the list.

##Week 2
###Common terms
* Mean == expected value of random variable??
* Mode == value with highest frequency
* Unimodal distribution has only one peak. Does that mean pdf or pmf are concave??

###Acquiring data
* Longitudinal studies -- acquiring data by following same subject for some time
* Cross sectional studies -- acquiring data by cross secting subjects at different age.

###Average vs. Median
* Median unaffected by outliers
* Right-skewed distribution (right hand tail) - average > median
* Left-skewed distribution (left hand tail)   - average < median
* percentile and averages does not necessarily relate. They depend on underlying distribution

###Markov inequality
In non-negative data sets, upper bound of values $\ge k\mu$ is $1/k$

###Measuring spread
* range
* IRQ - Interquartile range
* Standard Deviation (why n in formula for descriptive statistics and n-1 otherwise???)
###Chebychev Inequality
* Percent of proportion outside the range average ±k×SD is
at most 1/k^2 

##Week 3
###Normal curves 
* inflexions points and mu +- sd
* Need more information?? -proofs, common theorems and all that jazz. This section is rather week
* Tests whether distribution is normal?? How can I know which distribution fits best to the data??

##Week 4
###Bivariate data
* scatter plot
* vertical and horizontal slice
* vertical and horizontal scatter
* association: any relation between variables
* positive association: above average values of one variable tend to go with above average values of the other; the scatter slopes up
* negative association: above average values of one variable tend to go with below average values of the other; the scatter slopes down
* linear association: roughly, the scatter diagram is clustered around a straight linear
* Homoscedasticity and Heteroscedasticity
* football shaped.. is that multivariate gaussian??

###Correlation coefficient
* between -1 and 1
* invariant on coordinate axes and linear transformations (difference between affine and linear??)
* Need more proofs.
* simple formula => 1/n * dot product of z-scores of data. Maybe there is something more to this explanation??
* How to generate plot with given r??
* Ecological Correlation - clustering on averages (e.g. instead of student results taking into account state results) artificially increases correlation

###Linear regression
* minimizing rms error of estimate. $\sqrt(\frac{1}{n}\sum{(a*x_i + b - y_i)^2}$
* formula given as y (in standard units) = r * x (in standard units)
* I know usual calculus based approach in proving (without all the r business). Would like to see bit more detail 
* regression towards the mean
* regression fallacy

###Linear regression error
* rms error of regression line = sqrt(1-r^2) * sd(Y) irrelevant of scatter diagram
* Residual plot - differences between data and regression line (the best one)
	* average is 0
	* no linear association between residuals and x
	* Good regression: Residual plot looks like a formless blob around the horizontal axis.
	* Heteroscedasticity - different spread on residual plot
	* Outliers - unusually large positive or negative value on residual plot
	* Nonlinearity - residuals predominantly positive/negative on section of residual plot
