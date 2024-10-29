---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/data-analysis-in-transport-systems/diario-data-analysis-in-transport-systems/","tags":["UNI"]}
---

# [[Università/Magistrale/1° Anno/Data Analysis in Transport Systems/📊📔 Diario Data Analysis in Transport Systems\|📊📔 Diario Data Analysis in Transport Systems]]


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

[[Università/Magistrale/1° Anno/Data Analysis in Transport Systems/Notes/03 - Computational Statistical Inference - DATS\|03 - Computational Statistical Inference - DATS]]
- Contrast of hypothesis - Hypothesis testing
	- Level of significance
- Correlation between 2 numeric variables
	- Charts
	- Numbers
		- Pearson Correlation coefficient
		- Spearman's Correlation Coefficient
	- Test
		- `cor.test(X ~ Y)` - Person's test
		- `cor.test(X ~ Y, method = 'spearman')` - Person's test
- Correlation between a numeric variable and a factor (non numeric variable)
	- Charts
		- `boxplot(Y ~ A)`
	- Numbers
		- Coefficient of Determination $R^{2} \longleftarrow {\rm lm}(Y~A)$ (Linear Model)
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
- Correlation between 2 factors
	- Charts
		- mosaic plot - `plot(B~A)` You get mosaic plot automatically if it's 2 factos
	- Numbers
		- Contingency tables - `table(A,B)` --> `prob.table((A,B), 1)` or `prob.table((A,B), 2)`
	- Test
		- $\chi^{2}$ test - `chisq.test(B~A)`



