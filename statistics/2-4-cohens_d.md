[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

Exercise 2.4 Using the variable totalwgt_lb, investigate whether first ba-
bies are lighter or heavier than others. Compute Cohen's d to quantify the
difference between the groups. How does it compare to the difference in
pregnancy length?

First let's look at the mean's for first babies total weight against others (non-first born babies): 

```
firsts.totalwgt_lb.mean(), others.totalwgt_lb.mean()

(7.201094430437772, 7.325855614973262)
```
There is a slight difference and other babies are a bit heavier. 

Next step is to run the Cohen Effect Size formula to understand if this difference is signifcant. 

```
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)

-0.088672927072602006

```

The result is -.08. This is a very small measure. To compare, the Cohen Effect Size for pregnancy length is only .03, which is also quite small. Both results are far less than 1 standard deviation from the mean. 
