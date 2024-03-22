|Table 1|Table 2|Join by field(s)|
|------------------------|------------------------|-------------------------------|
csd_continuousDischarge|csd_gaugeWaterColumnRegression|regressionID
csd_continuousDischarge|sdrc_gaugePressureRelationship|Not fully automatable: Join by regressionID and endDate truncated to YYYY-MM-DD HH:MM (without seconds)
csd_continuousDischargeUSGS|csd_dischargeRegressionUSGS|usgsDischargeRegID
csd_continuousDischarge|csd_continuousDischargeUSGS|Join not possible
csd_continuousDischarge|csd_dischargeRegressionUSGS|Join not possible
csd_continuousDischargeUSGS|sdrc_gaugePressureRelationship|Join not possible