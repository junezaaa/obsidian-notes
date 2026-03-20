	 dispersion (การกระจายตัว) is how the data spread around the midpoint

- Metric 
	- Variance ความแปรปรวน
		- Deviation^2
		- Hard punished positive deviation
		- Deviation is the diff of a single data point from the mean, like how much the number deviate from the group typical score
		- var()
	- Standard Deviation
		- sqrt(variance) , all the deviation of the data
		- std()
	- Range Max-Min
		- percentile is the values the will put the value in the rank in percent
			- if x has a percentile of 20 , then 20% of the data is <= x, vice versa
	- IQR (inter-quartile range)
		- q3 - q1
		- To measure the dispersion
		- quantile()
		- percentile()

- Use boxplot to see the dispersion the box is 50% of the data the whisker is the rest (whisker may not be equal in range long tail short tail)
- ![[Pasted image 20260321023607.png|298]]
- Distance between Upper/Lower Extreme and Q3/Q1 is 1.5 x (q3-q1)

### Histogram
- Use histogram distplot() to show the amount of data of each type or where they are in each segment
- a graphical representation that organizes continuous data points into user-specified ranges (bins), displaying the **frequency distribution** via connected vertical bars

