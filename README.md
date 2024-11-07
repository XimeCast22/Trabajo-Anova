# Analisis de bacterias

> library(ggplot2)

> ggplot(bacteria_data) +
aes(x = Bacteria, y = rep1, color = Bacteria ) +
geom_jitter() +
theme(legend.position = "none")

![image](https://github.com/user-attachments/assets/e1122fa7-124f-47f2-9471-5f4858eccbe8)

ggplot(res_aov$residuals,
id = FALSE · id = FALSE to remove point identification
)

![image](https://github.com/user-attachments/assets/53cb8bb5-61e8-476f-844b-48755cecb258)


shapiro.test(res_aov$residuals)
  shapiro-wilk normality test

data: res_aov$residuals
w = 0.95831 ,  p-value = 0.2467

boxplot(rep1 ~ muestras,
     data = bacteria_data
)

![image](https://github.com/user-attachments/assets/d815494a-d6fd-49bd-b85c-d4debb816000)

ggbetweenstats(
data = bacteria_data,
x = muestras,
y = rep1,
type = "parametric",
var.equal = TRUE,
plot.type = "box",
pairiwise.comparisons = TRUE,
pairiwise.display = "significant",
centrality.plotting = FALSE,
bf.message = FALSE
)

![image](https://github.com/user-attachments/assets/b4dfe64f-b9a8-4865-89be-7780c98515d1)
