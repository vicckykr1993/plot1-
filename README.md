# plot1-
 house <- read.table("C:/Users/vicckykr1993/Desktop/house.txt", sep=";", quote="\"")
subset <- house[house$Date %in% c("1/2/2007","2/2/2007") ,]
globalActivePower <- as.numeric(subset$Global_active_power)
png("plot1.png", width=480, height=480)
hist(globalActivePower, col="blue", main="Global Active Power", xlab="Global Active Power (kilowatts)")
dev.off() 
