---
{"dg-publish":true,"permalink":"/catdes/"}
---

# [[catdes()\|catdes()]]

`catdes()` is a function provided in the [[FactoMineR\|FactoMineR]] package in [[R-Studio\|R-Studio]].

It performs categorical data description, analyzing relationship between a categorical variable (the *response*, or *target* variable) and all the other variables (*predictors*).

## Usage

Let there be a variable "hobbies"

```r
library(FactoMineR)

# Example dataset
data(hobbies)
result <- catdes(hobbies, num.var = 1)  # Variable 1 as the response
result

```

We use the function `catdes(hobbies, num.var = 1)`

The last command is telling to apply the catdes command to the variable "hobbies". It is also stating the target variable to be the first one: 1.

## Interpreting results

The `catdes()` function returns 4 kind of results that interest us, grouped in 4 variables.
- [[catdes()#$quanti.var\|#$quanti.var]]
- [[catdes()#$quanti\|#$quanti]]
- [[catdes()#$test.chi2\|#$test.chi2]]
- [[catdes()#$category\|#$category]]

### $quanti.var

The output of `catdes(...)` has been assigned to a variable named "result".

```r
result$quanti.var
```

The result will look something like this:

```console
$quanti.var
                 eta2      p.value
Sepal.Length    0.618     <2e-16
Sepal.Width     0.222      0.003
Petal.Length    0.930     <2e-16
Petal.Width     0.900     <2e-16
```

- Higher eta2 values mean greater correlation
- Lower p-value means greater significance of the eta2 value

So:
- Look for high eta2 with low p-values



### $quanti

### $test.chi2

### $category