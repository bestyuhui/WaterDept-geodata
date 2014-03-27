# GIS_WATER.PWD_PARCELS_rev

### Summary  

The primary purpose of PWD_PARCEL layer is to calculate parcel-based stormwater charges for PWD customers under the new parcel-based stormwater billing program.  The layer was created from the DOR_PARCELS layer in 2005 after it was decided that none of the other City parcel layers could meet the needs of PWD's stormwater billing program.  Those needs are generally that the parcel delineations match up to what people actually own, that there is an accurate assessment of the impervious area on the parcel, and that there is owner information associated with the parcel.  Over the past 5 years, PWD has made corrections based off deeds on file with DOR, BRT information, and other City records.  PWD also matched up each DOR parcel to a corresponding BRT record that contained the owner information for that parcel.

### Description  

ATTRIBUTE FIELDS:FIELD NAMEDATA TYPEDESCRIPTIONObject IDObject IDObject IDPARCELIDLong IntegerUNIQUE PARCELIDTENCODETextOPA TENCODEADDRESSTextADDRESSOWNER1TextOPA OWNER1OWNER2TextOPA OWNER2BLDG_CODETextOPA BLDG CODEBLDG_DESCTextOPA BLDG TYPE DESCRIPTIONBILLING_CLASSTextPROPERTY CLASSIFICATION USED IN BILLING A PARCEL FOR STORMWATER; EFFECTIVELY AN INTERPRETATION OF PWDS BILLING REGULATIONS AS APPLIED TO BLDG_DESCBRT_IDTextBRT TAX ACCOUNT IDNUM_BRTLong IntegerNUMBER OF OPA TAX ACCOUNTS IN PARCELNUM_ACCOUNTSLong IntegerNUMBER OF ACTIVE WATER ACCOUNTS IN PARCELSENSITIVE_CLASSTextFLAG TO FILTER OUT PROPERTIES OWNED BY A PARTICULAR ENTITY/GROUP; MAINTENANCE OF THIS FIELD IS SPORADICPARCEL_AREALong IntegerGROSS AREA OF PARCEL (IN SQ FT) AS CALCULATED FROM PARCEL POLYGON IN GISGROSS_AREALong IntegerTOTAL GROSS AREA OF PARCEL (IN SQ FT)IMPERV_AREALong IntegerTOTAL IMPERVIOUS AREA OF PARCEL (IN SQ FT)FINAL_GROSSLong IntegerGROSS_AREA, LESS ANY CREDITED GROSS AREA, ROUNDED UP TO NEXT 500 SQ FTFINAL_IMPERVLong IntegerIMPERV_AREA, LESS ANY CREDITED IMPERVIOUS AREA, ROUNDED UP TO NEXT 500 SQ FTMETER_CHARGEDoubleSUM OF ALL METERED-BASED STORMWATER CHARGES ON ALL ACTIVE WATER ACCOUNTS ON PARCEL; AMOUNT NO LONGER FACTORED INTO STORMWATER BILLING CHARGES, AS OF JULY 1, 2013.BRT_WEBSITETextURL OF OPA WEBSITE FOR PARCELS OPA TAX ACCOUNTSHAPE.AREADoubleAREASHAPE.LENDoubleLENGTHTo query for parcel vacancies, use the following SQL query in the BLDG_DESC field.SELECT * FROM PARCELS WHERE BLDG_DESC LIKE '%VAC%' in SQL orBLDG_DESC LIKE '%VAC%' in ARCMAP Select by Attribute window. The following categories are selected by the query.VAC LAND COMM. &lt; ACREVAC LAND COMM. ACRE+VAC LAND IND &lt; ACREVAC LAND INDUS. ACRE+VAC LAND RES &lt; ACREVAC LAND RESID. ACRE+VACANT LAND BILLBOARDNote that these are propoerties that are vacant (not developed), and not properties which are vacated (i.e. abandoned building). PARCELS layer doesn't have "Vacated property" information._________________________________________________________________________________________________________________________________________________________________________________ - Feature updated: 03/2014- Attributes updated: 03/2014- Metadata updated: 05/2013- Update Frequency: Monthly  

### Data Dictionary

| Field | Description  
| ----- | :----------:  
| FID |  
| Shape |  
| PARCELID |  
| TENCODE |  
| ADDRESS |  
| OWNER1 |  
| OWNER2 |  
| BLDG_CODE |  
| BLDG_DESC |  
| BILLING_CL |  
| BRT_ID |  
| NUM_BRT |  
| SENSITIVE_ |  
| NUM_ACCOUN |  
| PARCEL_ARE |  
| GROSS_AREA |  
| IMPERV_ARE |  
| FINAL_GROS |  
| FINAL_IMPE |  
| METER_CHAR |  
| BRT_WEBSIT |  
| SHAPE_AREA |  
| SHAPE_LEN |  


### Credits  

PWD GIS Unit/Stormwater Billing Unit Contact: Larry Szarek, PWD GIS Manager 1101 Market St Philadelphia PA 19107 215-685-6333

### Use Limitations  

The City of Philadelphia makes no representation about the accuracy of any specific information in this GIS data and is provided as is and without Warranty of any kind. Boundaries are self-reported. The user of this data will assume complete responsibility for any and all occurrences resulting from its use or display and will hold the City of Philadelphia harmless from any and all claims, demands, liabilities, obligations, damages, suits, judgments or settlements, including reasonable costs and attorneys' fees, that arise from use of this data.