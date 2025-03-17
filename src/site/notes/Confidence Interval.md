---
{"dg-publish":true,"permalink":"/confidence-interval/"}
---

# [[Confidence Interval\|Confidence Interval]]

A confidence interval is the interval in which a population statistic is contained when estimated by a sample statistic.

Let $\mu$ be some population mean of same value and let $\overline{X}$ be the mean of a sample of the population. Given an accuracy of $\alpha$ (s.t. the interval is accurate in $(1-\alpha) \%$ of cases), then a Confidence Interval for the population mean is:
$$
\mu \in \left[ \overline{X} - z_{1- \frac{\alpha}{2}} \frac{\sigma}{\sqrt{n}}; \overline{X} + z_{1- \frac{\alpha}{2}} \frac{\sigma}{\sqrt{n}}  \right]
$$
where $z_{1- \frac{\alpha}{2}}$ is the value of z (where z follows a [[Standard Normal Distribution\|Standard Normal Distribution]]) such that the area under the curve is equal to $1-\frac{\alpha}{2}$.

![Confidence Interval 2025-03-16 19.27.14.excalidraw.png](/img/user/Allegati/Confidence%20Interval%202025-03-16%2019.27.14.excalidraw.png)


We use the Standard normal distribution since is well known. Then, we scale it according to a factor dependent on the variance of the variable we are interested in: $\dfrac{\sigma}{\sqrt{n}}$.

```ad-example

One particular variable of a population has a mean of $\mu$ (unknown). We have a sample of the population with a mean for the same variable equal to $\overline{X}$. Let's suppose we know the population variance, $\sigma^{2}$. The sample is composed of $n$ elements.

We want an estimate for the population mean with 95% confidence. This mean we want an $\alpha=0.05$.

We are basically looking for the value:
$
z_{1- \frac{\alpha}{2}} = z_{1- \frac{0.05}{2}} = z_{1 - 0.025} = z_{0.975}
$
We want the value of $z$ such that the probability of that value is equal to 0.975.

From the probability table we can find out that such value is:
$
z = 1.960
$
given a large number of observations.
```

- $\alpha:$ [[Level of significance\|Level of significance]]
- The percentage is the [[Degree of confidence\|Degree of confidence]]

```ad-attention

We are assuming to know the variance of the population. This is clearly impossible. Actually, also the variance, as the mean, follows a random probability distribution (that can be proven to be a ???). For the porpuses we are usually interested in, we can simply use the sample variance ($s^{2}$) in place of the population variance.
```
