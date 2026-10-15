
There are three key concepts that act as the building blocks of data intensive applications. These are:

#### Reliability:

How reliable is a piece of software? Can it handle increased load and can it run efficiently under load.
#### Scalability:

Is a piece of software scalable? This includes both horizontal scaling (more machines), and vertical scaling (upgrading one machine). Scalable services can be elastic, meaning they can automatically scale at will, in response to real time load. 
#### Maintainability:

Can the system / software be upkept and adapted reliably, efficiently, and quickly? This is important in large applications such as X or Facebook.


Two units of measure for ensuring these:

- Average response time (for n inputs, add all n's and divide by number of n's)
- Percentiles. Amazon uses the 99.9th percentile as a target, as a 100ms increase in latency can lead to a 1% drop in total sales.