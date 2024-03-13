|Table 1|Table 2|Join by field(s)|
|------------------------|------------------------|-------------------------------|
dsc_fieldData|dsc_individualFieldData|namedLocation, collectDate when dsc_fieldData:DischargeBoutTypeID equals 'flowmeter' or 'flowmeter_rea'
dsc_fieldData|dsc_fieldDataADCP|namedLocation, collectDate when dsc_fieldData:DischargeBoutTypeID equals 'adcp' or 'adcp_rea'
dsc_fieldDataADCP|dsc_individualFieldData|Join not recommended: each table contains data for mutually exclusive discharge measurement methods