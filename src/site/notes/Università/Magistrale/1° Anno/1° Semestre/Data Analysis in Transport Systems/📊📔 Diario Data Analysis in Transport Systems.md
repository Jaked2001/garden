---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/data-analysis-in-transport-systems/diario-data-analysis-in-transport-systems/","tags":["UNI"],"dg-note-properties":{"aliases":["📊📔 Diario DATS"],"Tipo":"Diario","Materia":"DATS","Stato":null,"Parents":["[[📊 Data Analysis in Transport Systems|📊 DATS]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/📊📔 Diario Data Analysis in Transport Systems\|📊📔 Diario Data Analysis in Transport Systems]]


# 📆  15-10-2024 - Tue

### 📝 Theory

### ✏️ Projects


# 📆  22-10-2024 - Tue

### 📝 Theory

### ✏️ Projects


# 📆  24-10-2024 - Thu

LAB Session


# 📆  29-10-2024 - Tue

### 📝 Theory

[[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/03 - Computational Statistical Inference - DATS\|03 - Computational Statistical Inference - DATS]]
- Contrast of hypothesis - Hypothesis testing
	- Level of significance
- Correlation between 2 numeric variables - $(Y,X)$
	- Charts
	- Numbers
		- Pearson Correlation coefficient
		- Spearman's Correlation Coefficient
	- Test
		- `cor.test(X ~ Y)` - Person's test
		- `cor.test(X ~ Y, method = 'spearman')` - Person's test
- Correlation between a numeric variable and a factor (non numeric variable) - $(Y,A)$
	- Charts
		- `boxplot(Y ~ A)` or just use `plot(Y ~ A)`
	- Numbers
		- Coefficient of Determination $R^{2} \longleftarrow$ `lm(Y~A)` (Linear Model)
		- $eta^2$
	- Test
		- Test on means
			- j = 2
				- Parametric - Welch test: `t.test(Y~A)`
				- Non-parametric - Wilcoxon Test: `wilcox.test(Y~A)`
			- j > 2
				- Parametric - `oneway.test(Y~A)`
				- Non-parametric - `kruskal.test(Y~A)`
		- Test on variance
			- j = 2
				- Parametric - `var.test(Y~A)`
				- Non-parametric - `fligner.test(Y~A)`
			- j > 2
				- Parametric - `barlett.test(Y~A)`
				- Non-parametric - `fligner.test(Y~A)`
- Correlation between 2 factors - $(B,A)$
	- Charts
		- mosaic plot - `plot(B~A)` You get mosaic plot automatically if it's 2 factos
	- Numbers
		- Contingency tables - `table(A,B)` --> `prob.table((A,B), 1)` or `prob.table((A,B), 2)`
	- Test
		- Pearson's test on independence or $\chi^{2}$ test - `chisq.test(B~A)`





# 📆  31-10-2024 - Thu

### ✏️ Lab session

[[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/LabSess 3 - 2024-10-31 - Computational Statistical Inference - DATS\|LabSess 3 - 2024-10-31 - Computational Statistical Inference - DATS]]

We practiced all the tools introduced in the class of [[_Giornaliera/2024-10-29\|2024-10-29]] into RStudio.


# 📆  05-11-2024 - Tue

### 📝 Theory

[[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/03 - Computational Statistical Inference - DATS\|03 - Computational Statistical Inference - DATS]]
- `pariwise.t.test(Y,A)` - `pariwise.wilcox.test(Y~A)`
- `library(FactoMineR)`
	- `condes(df,'nb')` and `catdes(df,'nb')`
- ExTheo_5nov2024.Rmd example


# 📆  12-11-2024 - Tue

Preparation for Midterm.
Work in class on Midterm 2023-2024.


# 📆  14-11-2024 - Thu

- Preparation for Midterm.
	- Work in class on Midterm 2023-2024.
- Kyoto data analysis


# 📆  19-11-2024 - Tue

Midterm exam!


# 📆  26-11-2024 - Tue

### 📝 Theory

[[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/04 - Statistical modeling through regression - DATS\|04 - Statistical modeling through regression - DATS]]
- Linear models
	- Least square method


# 📆  28-11-2024 - Thu

### 📝 Theory

Lab session


# 📆  03-12-2024 - Tue


### 📝 Theory

[[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/04 - Statistical modeling through regression - DATS\|04 - Statistical modeling through regression - DATS]]
- Interpretation of `lm()` method output in [[R-Studio\|R-Studio]].
- Fisher test
	- 3 ways of defining the fisher test
- Testing multiple variables at the same time: `anova(submodel,Model)`
	- Output interpretation
	- Multiple correlation coefficient
- Prediction based on linear model
	- `predict(<model>, newdata=<dataframe>, interval = "prediction")`
- Model validation
	- `plot(<model>)` interpretation


# 📆  10-12-2024 - Tue

### 📝 Theory

[[Università/Magistrale/1° Anno/1° Semestre/Data Analysis in Transport Systems/Notes/04 - Statistical modeling through regression - DATS\|04 - Statistical modeling through regression - DATS]]
- Residuals
- Diagnostics
- Picking Best model


# 📆  12-12-2024 - Thu

Lab session on multiple linear regression.


# 📆  17-12-2024 - Tue

### 📝 Theory

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗
