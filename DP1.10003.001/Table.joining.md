|Table 1|Table 2|Join by field Table 1|Join by field Table 2|
|-----------------|----------------|-------------------------|--------------------|
brd_perpoint|brd_countdata|eventID, pointID|eventID, pointID|
brd_perpoint|brd_references|siteID, startDate|siteID, date|
brd_countdata|brd_identificationHistory|identificationHistoryID|identificationHistoryID
brd_countdata|brd_references|Join not recommended: References apply to entire observation period. Connect references to observations via siteID and dates.||
brd_personnel|Any other table|Join not recommended: Personnel are tested annually. To find relevant scores, measuredBy and technicianID fields match for the same observer, and test scores are relevant to data collected during the year of the test(s).||
