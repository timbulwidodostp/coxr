# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fit Robustly Proportional Hazards Regression Model Use coxr (coxrobust) With (In) R Software
install.packages("coxrobust")
library("coxrobust")
library("survival")
# Estimation Fit Robustly Proportional Hazards Regression Model Use coxr (coxrobust) With (In) R Software
coxr = read.csv("https://raw.githubusercontent.com/timbulwidodostp/coxr/main/coxr/coxr.csv",sep = ";")
coxr <- coxr(Surv(time, status) ~ coxr_1 + coxr_2 + coxr_3, data = coxr, trunc = 0.9)
coxr$coefficients
coxr$ple.coefficients
head(coxr$lambda, 3)
head(coxr$lambda.ple, 3)
head(coxr$var, 1)
head(coxr$var.ple, 1)
coxr$wald.test
coxr$ewald.test
# Fit Robustly Proportional Hazards Regression Model Use coxr (coxrobust) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished