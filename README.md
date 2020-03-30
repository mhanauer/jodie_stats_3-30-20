---
title: "Test"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

Jodie results
```{r}
time_point = c(1:6)
score = c(3,5,5.6, 6, 6.5, 6.8)
dat_jodie = cbind(time_point, score)
library(lmtest)
dw_lm = lm(score ~ time_point)
dwtest(dw_lm)
```

