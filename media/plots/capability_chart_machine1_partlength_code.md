# R Code for Machine 1 Process Capability (PartLength)
data_M1_cap <- X037[X037$Machine == 1 & X037$Temperature == 338 & X037$Pressure == 200, ]
LSL <- 45; USL <- 55; Target <- 50
qcc_object_M1_cap <- qcc(data_M1_cap$PartLength, type = "xbar.one", plot = FALSE)
cap_M1_summary <- capture.output(process.capability(qcc_object_M1_cap, spec.limits = c(LSL, USL), target = Target))
png("media/plots/capability_chart_machine1_partlength.png", width = 800, height = 600)
process.capability(qcc_object_M1_cap, spec.limits = c(LSL, USL), target = Target)
dev.off()
