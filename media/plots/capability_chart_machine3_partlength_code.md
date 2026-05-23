# R Code for Machine 3 Process Capability (PartLength)
data_M3_cap <- X037[X037$Machine == 3 & X037$Temperature == 338 & X037$Pressure == 200, ]
LSL <- 45; USL <- 55; Target <- 50
qcc_object_M3_cap <- qcc(data_M3_cap$PartLength, type = "xbar.one", plot = FALSE)
cap_M3_summary <- capture.output(process.capability(qcc_object_M3_cap, spec.limits = c(LSL, USL), target = Target))
png("media/plots/capability_chart_machine3_partlength.png", width = 800, height = 600)
process.capability(qcc_object_M3_cap, spec.limits = c(LSL, USL), target = Target)
dev.off()
