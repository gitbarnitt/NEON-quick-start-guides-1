|Table 1|Table 2|Join by field(s)|
|------------------------|------------------------|-------------------------------|
bbc_percore|bbc_rootmass|sampleID
bbc_percore|bbc_dilution|sampleID
bbc_rootmass|bbc_chemistryPooling|Not fully automatable: multiple subsampleIDs are pooled into each subsampleIDList
bbc_chemistryPooling|bbc_rootChemistry|cnSampleID
bbc_chemistryPooling|bbc_dilution|Requires intermediate table: join via bbc_rootmass table
bbc_chemistryPooling|bbc_percore|Requires intermediate table: join via the bbc_rootmass table
bbc_chemistryPooling|bbc_rootChemistry|cnSampleID
bbc_dilution|bbc_rootChemistry|Requires intermediate table: join via the bbc\_rootmass and bbc\_chemistryPooling tables
bbc_dilution|bbc_rootmass|Not fully automatable: need to calculate mean fragmentDryMass in bbc_dilution and sum of size classes in bbc_rootmass before joining by sampleID (see Standard calculations in Quick Start Guide)
bbc_percore|bbc_rootChemistry|Requires intermediate table: join via the bbc\_rootmass and bbc\_chemistryPooling tables
bbc_rootChemistry|bbc_rootmass|Requires intermediate table: join via the bbc_chemistryPooling table
bgc\_CNiso\_externalSummary|Any other table|Join not recommended. Data resolution does not match other tables.
