[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> REPLACE THIS TEXT WITH YOUR RESPONSE

import scipy.stats

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)



print(dist.cdf(177.8))
print(dist.cdf(185.4))
print("The percentage of US male population in this range is: ", round(abs(dist.cdf(185.4) - dist.cdf(177.8)), 4)*100)


output:
0.48963902786483265
0.8317337108107857
The percentage of US male population in this range is:  34.21