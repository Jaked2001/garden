---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/data-analysis-in-transport-systems/notes/04-statistical-modeling-through-regression-dats/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/04 - Statistical modeling through regression - DATS\|04 - Statistical modeling through regression - DATS]]

References:
- Fox, J, Applied Regression Analysis and Generalized Linear Models, Sage Publications

```ad-danger

These notes are not intended for a deep understanding of the topic. They are just a guide to try and survive the [[📊 Data Analysis in Transport Systems|📊 DATS]] exam.

They contain no rigor and may contain mistakes.
```

The goal is to model a target (or response) variable, $\mathbf{Y}$ as a linear combination of some exploratory variables, $\mathbf{X}$. More precisely, we will obtain a prediction of the target, $\boldsymbol{\eta}$. 
$$
\boldsymbol{\mu} = \boldsymbol{\eta} = \mathbf{X} \boldsymbol{\beta}
$$
- $\boldsymbol{\beta}$ is the vector of coefficients.
- $\mathbf{X}$ is a matrix where each column is an exploratory variable. The first column is just 1s.
$\eta$ only describes the systemic component.
The vector $\eta$ has the same length as the target variable.

Part of the variability of the response is not describied in $\boldsymbol{\eta}$, so, to get $\mathbf{Y}$ we also need to add the remaining part, known as **residuals**: $\boldsymbol{\varepsilon} = \mathbf{e_{i}} = \mathbf{Y_{i}} - \mathbf{\hat{Y}_{i}}$. $\mathbf{\hat{Y}_{i}}$ is the prediction of the response according to the model.

$\boldsymbol{\beta}$ is a list of coefficients:
$$
\boldsymbol{\beta} = \beta_{1}, \beta_{2}, ..., \beta_{n}
$$
where $n$ is the number of variables and $\beta_{1}$ is known as the **intercept**.

To summarise:
$$
\mathbf{Y} = \boldsymbol{\mu} + \boldsymbol{\varepsilon} = \mathbf{X}\boldsymbol{\beta } + \boldsymbol{\varepsilon}\mathbf{}
$$

# Model in R

If all exploratory variables are numeric, the process is quite simple. The rules described above all stand.

In R-studio we proceed as follows:
- Y: target variable
- X1, X2, ..., Xp: All the exploratory variables (There are a number p of them)

```{R}
m1 <- lm(Y ~ X2 + X3 + ... + Xp)
summary(m1)
```

Then we do a summary of the model

![04 - Statistical modeling through regression - DATS 2025-01-09 16.54.29.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Data%20Analysis%20in%20Transport%20Systems/Notes/Allegati/04%20-%20Statistical%20modeling%20through%20regression%20-%20DATS%202025-01-09%2016.54.29.excalidraw.png)


**FISHER-ANOVA:**
We can try making a new model with less variables. 
Let $M$ be the original complete model. Then we can make $m$ a nested model of $M$ (It has the same form of $M$ but with less variables).

We can use the **FISHER** test to verify if the 2 models are equivalent. If they are, it's better to use the smaller one.

Fisher test: H0 = Models m and M are equivalent
- $p\gg0.05$ Accept H0
- $p\ll0.05$ Reject H0 --> Need to use big model M

In R studio this test is done using the function `anova(m1,m2)`

```{R}
anova(m1, m2)
```

Read p-value of the test.

If using glm(), then use the Wald test

## Unusual and influential data

**Regression outlier**: observation with unusual value of the outcome variable Y, conditioned by the value of the explanatory variable X.

**LEVERAGE**
- An observation with high leverage has an unusual X value and has leverage on the regression line.
- Leverage is higher for an observation further away from the mean of X
- If the value has high leverage but still fall onto the regression line, this is not a problem as it does not influence the regressio coefficients

**INFLUENTIAL OBSERVATIONS:**
- If an observation has high leverage and also falls far from the regression line, then is considered influential.
- It has unsual X value and Y value

`influencePlot()` can give what are the most influential observations:

```{R}
influencePlot(m1, pch=19, id = list(method="noteworthy", n=3))
```

OUTPUT:

![04 - Statistical modeling through regression - DATS 2025-01-11 17.04.16.excalidraw.png](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Data%20Analysis%20in%20Transport%20Systems/Notes/Allegati/04%20-%20Statistical%20modeling%20through%20regression%20-%20DATS%202025-01-11%2017.04.16.excalidraw.png)








