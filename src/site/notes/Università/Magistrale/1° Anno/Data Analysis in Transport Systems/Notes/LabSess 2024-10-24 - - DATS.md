---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/data-analysis-in-transport-systems/notes/lab-sess-2024-10-24-dats/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Data Analysis in Transport Systems/Notes/LabSess 2024-10-24 - - DATS\|LabSess 2024-10-24 - - DATS]]

Read file with command

`sample <-read.csv("Data38 Lab Session.txt",header=T,sep="",dec=".")`

make an histogram:

`hist(sample$x)`

Calculate mean and standard deviation:

Make a manual QQ plot. against a theoretical distribution. In this case, normal.

```R

# QQ plot against a standard normal distribution 
xx <- qnorm( ppoints( sample$x ))
yy<- sort( sample$x )
mm <- lm( yy ~ xx )
cor(yy,xx) # Squared correlation coeff is R2
plot( xx, yy, main="QQPlot") # plot std theo vs obs ptiles
lines( xx, mm$fitted.values, col=2 )
summary(mm)
```


The data has been uploaded as a data frame of one column. Everytime we need the data, we have to call it like sample$x (get column x from sample file).

Make it a vector (list, without names) on it's own:

`mysample <- sample$x`


Comment several lines: cmd+shift+c

Check for auto-correlation with acf:
`acf(wsample)  # OK no correlation: checked through the autocorrelation function`

![Auto corrletaion Function check.png](/img/user/Auto%20corrletaion%20Function%20check.png)

a pattern like this, means that it is not autocorrelated.

## Fitting process

### Exponential

```R
# ML Estimation:
## MASS library

me1<-fitdistr(uwsample,"exponential",lower=0.0001)
me1

## fitdistrplus

fe1<-fitdist(uwsample,"exp")
plot(fe1)
summary(fe1)

```

from the second command, we get:

![fitdist - Exponential.png](/img/user/fitdist%20-%20Exponential.png)


### Weibull

```r
# ML Estimation:
## MASS library

me2<-fitdistr(uwsample,"weibull",lower=0.001)
me2

## fitdistrplus

fe2<-fitdist(uwsample,"weibull")
plot(fe2)
summary(fe2)

```

We get these plots:

![fitdist - Weibull.png](/img/user/fitdist%20-%20Weibull.png)

This is closer than the [[Università/Magistrale/1° Anno/Data Analysis in Transport Systems/Notes/LabSess 2024-10-24 - - DATS#Exponential\|#Exponential]] but still, the tails do not match.

The summary of the distribution gives:

Fitting of the distribution ' weibull ' by maximum likelihood 
Parameters : 
       estimate Std. Error
shape  2.372017 0.02861668
scale 11.315081 0.08239124
Loglikelihood:  -10766.42   AIC:  21536.83   BIC:  21549.29 
Correlation matrix:
          shape     scale
shape 1.0000000 0.3254611
scale 0.3254611 1.0000000

### Gamma

Now we try the Gamma distribution

```r
# ML Estimation:
## MASS library

me3<-fitdistr(uwsample,"gamma",lower=0.001)
me3

## fitdistrplus

fe3<-fitdist(uwsample,"gamma")
plot(fe3)
summary(fe3)

```

![fitdist - Gamma.png](/img/user/fitdist%20-%20Gamma.png)

These are the parameters:

Fitting of the distribution ' gamma ' by maximum likelihood 
Parameters : 
       estimate Std. Error
shape 5.0105617 0.11207122
rate  0.5002168 0.01176835
Loglikelihood:  -10677.34   AIC:  21358.67   BIC:  21371.13 
Correlation matrix:
          shape      rate
shape 1.0000000 0.9507085
rate  0.9507085 1.0000000


The AIC and BIC values are smaller than the values in Wibull

# Validation

Combine all the criteria:
- Graphic (all the plots)
- Number (compare theoretical and sample's moments)
- Inferential