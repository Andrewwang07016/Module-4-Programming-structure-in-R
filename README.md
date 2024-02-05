# Module-4-Programming-structure-in-R

# Set variables
Freq <- c(0.6, 0.3, 0.4, 0.4, 0.2, 0.6, 0.3, 0.4, 0.9, 0.2)
bloodp <- c(103, 87, 32, 42, 59, 109, 78, 205, 135, 176)
first <- c(1, 1, 1, 1, 0, 0, 0, 0, NA, 1)
second <- c(0, 0, 1, 1, 0, 0, 1, 1, 1, 1)
finaldecision <- c(0, 1, 0, 1, 0, 1, 0, 1, 1, 1)

LocalHospital <- data.frame(Freq, bloodp, first, second, finaldecision)
LocalHospital

# Sets the layout of boxplot 1 row 2 columns
par(mfrow = c(1,2))

boxplot(LocalHospital$Freq)
boxplot(LocalHospital$bloodp)

hist(LocalHospital$Freq)
hist(LocalHospital$bloodp)

