|Table 1|Table 2|Join by field(s)|
|------------------------|------------------------|-------------------------------|
inv_fieldData|inv_persample|sampleID
inv_persample|inv_taxonomyRaw|sampleID
inv_persample|inv_taxonomyProcessed|sampleID
inv_fieldData|inv_taxonomyRaw|sampleID
inv_fieldData|inv_taxonomyProcessed|sampleID
inv_taxonomyRaw|inv_taxonomyProcessed|Join not recommended. If interested in processed NEON vs. raw lab taxonomy, join by sampleID + scientificName + sizeClass.
inv_fieldData|inv_pervial|sampleID
inv_persample|inv_pervial|sampleID
inv_taxonomyRaw|inv_pervial|Join not recommended. Data resolution does not match other tables.
inv_taxonomyProcessed|inv_pervial|Join not recommended. Data resolution does not match other tables.
