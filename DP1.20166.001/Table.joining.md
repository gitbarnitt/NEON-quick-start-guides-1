|Table 1|Table 2|Join by field Table 1|Join by field Table 2|
|------------------------|------------------------|-------------------------------|-------------------------------|
alg_fieldData|alg_biomass|parentSampleID|parentSampleID
alg_fieldData|alg_biomassComp|compositeSampleID|compositeSampleID
alg_biomass|alg_taxonomyProcessed|sampleID|sampleID
alg_biomassComp|alg_taxonomyProcessedComp|analyteSampleID|sampleID
alg_biomass|alg_taxonomyRaw|sampleID|sampleID
alg_biomassComp|alg_taxonomyRawComp|analyteSampleID|sampleID
alg_fieldData|alg_taxonomyProcessed|Requires intermediate table: join via alg_biomass table
alg_fieldData|alg_taxonomyProcessedComp|Requires intermediate table: join via alg_biomassComp table
alg_fieldData|alg_taxonomyRaw|Requires intermediate table: join via alg_biomass table
alg_fieldData|alg_taxonomyRawComp|Requires intermediate table: join via alg_biomassComp table
alg_qualityCheck|alg_taxonomyProcessed|sampleID, algalAnalysisMethod|sampleID, algalAnalysisMethod
alg_qualityCheck|alg_taxonomyRaw|sampleID, algalAnalysisMethod|sampleID, algalAnalysisMethod
alg_taxonomyProcessed|alg_taxonomyRaw|Join not recommended. These tables contain identifications of the same samples with possibly differing higher-order taxonomy; see User Guide.
alg_taxonomyProcessedComp|alg_taxonomyRawComp|Join not recommended. These tables contain identifications of the same samples with possibly differing higher-order taxonomy; see User Guide.
alg_taxonomyProcessedComp|alg_voucherTaxonomy|scientificName, voucherFloraVersion|scientificName, voucherFloraVersion
alg_taxonomyRawComp|alg_voucherTaxonomy|scientificName, voucherFloraVersion|scientificName, voucherFloraVersion
alg_taxonomyProcessedComp|alg_slideLocations|slideID|slideID
alg_taxonomyRawComp|alg_slideLocations|slideID|slideID
alg_archive|Any other table|Join not recommended. This table is an account of subsamples shipped to the biorepository.
alg_biovolumes|Any other table|Join not recommended. Data resolution does not match other tables.
