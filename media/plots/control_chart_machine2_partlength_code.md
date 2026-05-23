# R Code for Machine 2 Control Chart (PartLength)
data_M2_ctrl <- X037[X037$Machine == 2 & X037$Temperature == 338 & X037$Pressure == 200, ]
qcc_object_M2_ctrl <- qcc(data_M2_ctrl$PartLength, type = "xbar.one", plot = FALSE)
png("media/plots/control_chart_machine2_partlength.png", width = 800, height = 600)
plot(qcc_object_M2_ctrl, title = "Machine 2 Control Chart (PartLength)",
     xlab = "Observation", ylab = "PartLength",
     bg.lab = "#f0f0f0", cex.axis = 1.2, cex.lab = 1.2, cex.main = 1.5)
dev.off()
