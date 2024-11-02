---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/data-analysis-in-transport-systems/notes/lab-sess-1-2024-10-03-introduction-to-r-studio-dats/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Data Analysis in Transport Systems/Notes/LabSess 1 - 2024-10-03 - Introduction to RStudio - DATS\|LabSess 1 - 2024-10-03 - Introduction to RStudio - DATS]]

Files:
- [[Lab1 3 Oct 2024.r\|Lab1 3 Oct 2024.r]]
- [[Lab1 3 Oct 2024.rmd]]

Set working directory. Options:
- Write command
- Use interface

# Setup

## Comments

```R

```

## Set directory

To set the directory through code, use `setwd()`

```R
setwd("~/Library/Mobile Documents/com~apple~CloudDocs/0_MATTEO/0_School/0_Università/1_Magistrale/1_UPC - Barcellona/1° Year/Data Analisys in Transport Systems/Lab Sessions/2024-10-03 - DATS")
```

## Packages

Can add packages through code:

```R
library(car)
library(AER)
```

but have to also check it in the "Packages" section

If a package doesn't appear, go to
Install > "write the name" > Install

## Run

### Run 1 line or selection

Put pointer to 1 line, or select the line

Click: `Run the current line or selection` (Cmnd + Enter)

## Inport data

```R
data(name of data)
```

### View data

To write in console

```R
View(name of data)
```

this isn't efficient with very big data frames.

## Help

Run:

```
?"Name of command"
```

Running a command with a "?" before, opens the "help" section. You can also do it for data.


# Univariate Explorative Data Analysis

**Univariate:** Understand variables one-by-one.


## Numeric Indicators

Use `summary(Davis)`:
- Gives basic statistics:
	- min
	- max
	 - 1st Quartile
	- Median (2nd Quartile)
	- 3rd Quartile
	- Mean

**Factor:** term in R for a qualitative variable (has label). ie, M/F (Male or Female). In this case, `summary()` just counts...

## Charts

We'll first see basic charts for 1 variable

### Charts for factors

Factors:
Possible charts:
- Barplot
- Piechart

The variable "sex" only exists as a column of Davis. It is NOT an object. R can only work with objects.

We can select a part of an object using a Dollar symbol (\$).
ie:
```R
# Give summary of the variable "sex" in "Davis"
summary(Davis$sex)
```

We need tables, w/ command `table`: it counts the number if observations for each label.

```R
# Give summary of the variable "sex" in "Davis"
table(Davis$sex)
```

To assign a name to something, we can use the = sign, or the <- arrow.

```R
# the following commands, give the name tt to the table

tt <- table(Davis$sex)

# or

tt = table(Davis$sex)
```

Charts in R are ugly. To make them beautiful we can use a package ggplot2


#### Barplot

```R
barplot()
barplot(tt,main="My first barplot")
barplot(tt,main="My first barplot",col="cyan")
barplot(tt,main="My first barplot",col=heat.colors(2))
```

#### Pie chart

```R
pie(tt) # Make a pie chart
```

### Charts for num variables

#### Histogram

It has beams, not bars

```R
hist(Davis$height) # Makes an histogram
hist(Davis$height,main="My first Histogram",col="magenta") # Make title and color
```

```R
# Higher customization

hist(Davis$height,10,main="My first Histogram",col="magenta") # Make histogram dividing the range into 10 intervals (10 beams) of the same lenght


hist(Davis$height,breaks=seq(50,200,5),main="My first Histogram",col="magenta") # From 50 to 200, the lenght of the beam is equal to 5
```

if I use `freq= F` (F = False), it means that I'm not interested to the absolute number of observations, but to the ???

Applying a distribution to a set of data:

```R
hist(Davis$height,freq=F,breaks=seq(50,200,5),main="My first Histogram",col="magenta")
mm<-mean(Davis$height);ss<-sd(Davis$height);mm;ss # Calculate mean and Standard Deviation (needed for the density func of the normal distrib.) and assign them to variables called mm and ss
curve(dnorm(x,mm,ss),add=T,col="blue",lwd=2) # Applies the normal distribution using the mean mm and the Standard Deviation ss
# In the last command: dnorm() is the normal distribution, "add=T"R

```

We can do a test to check. For example the [[Università/Magistrale/1° Anno/Data Analysis in Transport Systems/Notes/Shapiro Wilk test\|Shapiro Wilk test]].