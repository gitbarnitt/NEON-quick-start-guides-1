|Table 1|Table 2|Join by field(s)|
|------------------------|------------------------|-------------------------------|
alg_fieldData|alg_biomass|parentSampleID
alg_biomass|alg_taxonomyProcessed|sampleID
alg_biomass|alg_taxonomyRaw|sampleID
alg_fieldData|alg_taxonomyProcessed|Requires intermediate table: join via alg_biomass table
alg_fieldData|alg_taxonomyRaw|Requires intermediate table: join via alg_biomass table
alg_qualityCheck|alg_taxonomyProcessed|sampleID, algalAnalysisMethod
alg_qualityCheck|alg_taxonomyRaw|sampleID, algalAnalysisMethod
alg_taxonomyProcessed|alg_taxonomyRaw|Join not recommended. These tables contain identifications of the same samples with possibly differing higher-order taxonomy; see User Guide.
alg_archive|Any other table|Join not recommended. This table is an account of subsamples shipped to the biorepository.
alg_biovolumes|Any other table|Join not recommended. Data resolution does not match other tables.
