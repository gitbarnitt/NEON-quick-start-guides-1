|Table 1|Table 2|Join by field(s)|
|------------------|-------------------|--------------------|
asc_fieldDataStation|asc_fieldDataZone|sedimentSampleID|
asc_fieldDataStation|asc_fieldDataPoint|sedimentSampleID|
asc_fieldDataStation|asc_externalLabData|Not fully automatable: sampleID in asc\_externalLabData corresponds to carbonSedimentSampleID, organicSedimentSampleID, and inorganicSedimentSampleID in asc\_fieldDataStation|
asc_externalLabData|asc_fieldDataPoint|Requires intermediate table: join via asc_fieldDataStation table|
asc_externalLabData|asc_fieldDataZone|Requires intermediate table: join via asc_fieldDataStation table|
asc_fieldDataPoint|asc_fieldDataZone|sedimentSampleID|
asc_externalLabSummary|Any other table|Join not recommended. Match by laboratoryName, analyte, method, and overlap of analysisDate with externalLabSummary dates.|
