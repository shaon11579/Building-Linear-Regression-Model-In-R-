# Building-Linear-Regression-Model-In-R-

# June 13

June13 <- read.csv("GDCm13.CSV", TRUE, ",")
summary(June13)
names(June13)



# regression 13

Regression13 <- lm(INV.Growth ~  Safety.Stock + Forecasting.Bias, data = June13)
summary(Regression13)
 # RM2
Regression13.1 <- lm(INV.Growth ~ Forecasting.Bias, data = June13)
summary(Regression13.1)

# RG Model 
Regression13.all <- lm(INV.Growth ~ Forecasting.Bias+FCST_1_ID + X11.09.2018.INV+ Safety.Stock +Demand.Type+Safety.2,  data = June13)
summary(Regression13.all)

# RG 2

Regression13.2 <- lm(INV.Growth ~ Forecasting.Bias+FCST_1_ID + X11.09.2018.INV+ Safety.Stock +Safety.2,  data = June13)

summary(Regression13.2)


# RG3

Regression13.3 <- lm(INV.Growth ~ Forecasting.Bias+FCST_1_ID + X11.09.2018.INV+ Safety.Stock,  data = June13)

summary(Regression13.3)



# RG4


Regression13.4 <- lm(INV.Growth ~ Forecasting.Bias + Safety.Stock,  data = June13)

summary(Regression13.4)

head(June13)

# RG5

Regression13.5 <- lm(INV.Growth ~ Forecasting.Bias + Safety.Stock+FCST_1_ID + Demand.Type + Safety.2,  data = June13)

summary(Regression13.5)

# RG6

Regression13.6 <- lm(INV.Growth ~ Forecasting.Bias + Safety.Stock+FCST_1_ID ,  data = June13)

summary(Regression13.6)



# RG7

Regression13.7<- lm(INV.Growth ~ Forecasting.Bias + Safety.2 +FCST_1_ID ,  data = June13)

summary(Regression13.7)





