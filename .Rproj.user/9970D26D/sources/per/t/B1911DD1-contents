#Data visualization project using cancer patient data from Denmark

# ---- Load libraries and data ----
install.packages("tidyverse")
library(tidyverse)
data <- read_csv("cancer_data_denmark.csv")
head(data)

# ---- Explore data with basic plots ----
#bar plot of cancer types
plot_cancer_type <- ggplot(data, aes(x = Cancer_Type)) + geom_bar(fill = "skyblue") + coord_cartesian(ylim = c(425,525)) + labs(title = "Cancer Type Distribution", x = "Cancer Type", y = "Count") + theme_minimal()
ggsave("plots/cancer_type_distribution.png", plot = plot_cancer_type, width = 8, height = 6, dpi = 300, bg = "white")


#density plot of age
plot_age <- ggplot(data, aes(x=Age)) + geom_density(fill="skyblue", color = "darkblue", alpha=0.4) + scale_x_continuous(limits = c(0,100), breaks = seq(0, 100, 20)) + labs(title = "Age Distribution of Cancer Patients", x = "Age", y = "Density") + theme_minimal()
ggsave("plots/age_distribution.png", plot = plot_age, width = 8, height = 6, dpi = 300, bg = "white")



