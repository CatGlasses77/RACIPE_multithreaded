RACIPE_multithreaded is a modification of RACIPE-1.0 (https://github.com/simonhb1990/RACIPE-1.0). RACIPE_multithreaded is capable of using multiple threads to perform computation unlike RACIPE-1.0, which lead to significant speed boosts.

The input and output data is the same as RACIPE-1.0, but there's an additional input (-threads <number>) that controls the number of threads used. We have observed an exponential like plot for number of threads vs time taken here, so you might want to try out some values of threads before running models. The time difference becomes very negligible as the number of threads grows larger, so make sure to get enough data points.
	
On testing this on a 12 core CPU, we found that using 80 threads gave a speed boost of about 12 times in comparison to the default RACIPE version.
