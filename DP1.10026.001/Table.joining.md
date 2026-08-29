|Table 1|Table 2|Join by field(s)|Notes|
|-----------------|-----------------|----------------|--------------------|
cfc_fieldData|cfc_chemistrySubsampling|sampleID||
cfc_fieldData|cfc_chlorophyll|sampleID||
cfc_fieldData|cfc_carbonNitrogen|sampleID||
cfc_fieldData|cfc_elements|sampleID||
cfc_fieldData|cfc_lignin|sampleID||
cfc_fieldData|cfc_LMA|sampleID||
cfc_fieldData|vst_mappingandtagging|individualID|Use a left join for these tables; most tagged plants have not been sampled for foliage. If using neonOS::joinTableNEON(), include input parameter location.fields=FALSE|
cfc_carbonNitrogen|cfc_chemistrySubsampling|sampleID||
cfc_carbonNitrogen|cfc_chlorophyll|sampleID||
cfc_carbonNitrogen|cfc_elements|sampleID||
cfc_carbonNitrogen|cfc_lignin|sampleID||
cfc_carbonNitrogen|cfc_LMA|sampleID||
cfc_chemistrySubsampling|cfc_chlorophyll|sampleID||
cfc_chemistrySubsampling|cfc_elements|sampleID||
cfc_chemistrySubsampling|cfc_lignin|sampleID||
cfc_chemistrySubsampling|cfc_LMA|sampleID||
cfc_chlorophyll|cfc_elements|sampleID||
cfc_chlorophyll|cfc_lignin|sampleID||
cfc_chlorophyll|cfc_LMA|sampleID||
cfc_elements|cfc_lignin|sampleID||
cfc_elements|cfc_LMA|sampleID||
cfc_lignin|cfc_LMA|sampleID||
bgc\_CNiso\_externalSummary|Any other table|Join not recommended. Data resolution does not match other tables.||
cfc_chlorophyllParameters|Any other table|Join not recommended. Data resolution does not match other tables.||
cfc_chlorophyllSummary|Any other table|Join not recommended. Data resolution does not match other tables.||
cfc_elementsSummary|Any other table|Join not recommended. Data resolution does not match other tables.||
lig_externalSummary|Any other table|Join not recommended. Data resolution does not match other tables.||
cfc_shapefile|Any other table|Join not recommended. This table provides metadata about canopy perimeter shapefiles collected during sampling.||
