# Data Management Plan

## Data Description
The example provided for the “LTREB: Drivers of temperate forest carbon storage from canopy closure through successional time” seemed very straight forward, so I will emulated that. I plan on producing three types of data:

a.	Physical samples: These samples will be collected pre and post restoration treatment and will include soil and root samples. The soil samples will have a bulked soil component, while the other will be cold stored and processed to determine mycorrhizal populations. Each sample will be save based on a numerical system associated to each plot.

b.	Field observations: Pre-restoration the GPS location, elevation, soil series evaluation, parent material, plant species, soil/air temperatures and humidity will be documented for each plot. Post-restoration, these same observations will be documented, along with stress monitoring for planted species. Stress monitoring will look for signs of desiccation, disease, predation, or death. These data will be documented on hard copy data sheet, which will be digitalized as PDF/As. They will then be complied for examination after the experimental time is complete. 

c.	Laboratory data: A combination of hard copy and digital data sets will record the soil laboratory analysis outputs, which will include mass, nutrient content (nitrogen, phosphorus, potassium, and carbon content). The mycorrhizal samples from the soil and roots will have the amplified RNA sequence of the 18S gene (the typical gene sequence for fungi). They will be complied and compared to the datasets existing in the “Basic Local Alignment Search Tool (BLAST)” from the National Center for Biotechnology Information to determine the mycorrhizal populations for each plot and root association.

For each data type the amount of data generated will be as follows:

a.	Physical samples: 50 MB

b.	Field observations: 50 MB

c.	Laboratory data: upwards of 1 TB depending on how many mycorrhizal RNA sequences are present. 

## Roles and Responsibilities
•	The final responsibility for data management, which includes DMP implementation, data organization, quality control, metadata generation, and data archiving rests with the Master’s student, G. Patty. Patty is also responsible for data dissemination once the final products are produced.

•	Data collection is the primary responsibility of Patty, but additional data collection help and research area maintenance will be shared with the senior field manager of Clean Water Services, J. Goetz, and possibly a field technician. 

•	Laboratory analysis and instrument maintenance will be the primary responsibility of Patty, with additional direction from Hatten Soils Lab manager I and the Biodeterioration Lab Senior Faculty Research Assistant. Patty will receive help with the soil samples determining the bulked soil mass and the nutrient contents in the Hatten lab, while in the Biodeterioration Lab, mycorrhizal samples will be processed for DNA sequencing.

•	Data and statistical analysis is the responsibility of Patty, but much direction will be provided by the College of Forestry’s statistician. 

•	If someone were to leave the project, the research would likely fall upon the senior field manager for Clean Water Services, as they own the land and they are funding the research. This may also mean the research becomes proprietary data for Clean Water Services unless they find another graduate student. 

•	There are no data sharing requirements, non-disclosure agreements, nor sensitive and confidential data generate by this project. The goals of this projects are increase the scope and success of restoration by sharing the results with anyone engaged in restoration, both for profit and non-profit groups.

## Data Standards and Metadata
1)	As described in the “Data Description” portion of the DMP, I will generate three types of data: physical samples, field observations, laboratory data.

a.	Physical samples: the physical soil samples will be created in the field for later evaluation in the lab. There will be four sample types,  two for soil condition evaluation, and two for mycorrhizal RNA 18S sequencing. The samples will be titled as follows, first for pre-restoration, then post:

i.	Patty_Pre_sitelocation_plotnumber_datecollected(dd/mm/yyyy)

ii.	Patty_Pre_mycor_sitelocation_plotnumber_datecollected(dd/mm/yyy)

i.	Patty_Post_sitelocation_plotnumber_datecollected(dd/mm/yyyy)

ii.	Patty_Post_mycor_sitelocation_plotnumber_datecollected(dd/mm/yyyy)

b.	Field and soil condition observations: This data will be recorded tabularly on site to then be digitized into Excel to match the soil condition file names above. The bolded headings will be recorded in lab and added to the digitized sheets. 

i.	Restoration level (pre or post)

ii.	Location: GPS coordinates

iii.	Elevation

iv.	Soil Temperature

v.	Soil humidity

vi.	Soil nutrients: nitrogen, phosphorus, potassium

vii.	Soil texture

viii.	Plant species on site

ix.	Plant stress indicators 

x.	Bulk density = dry weight/volume (to determine compaction)

xi.	Fine fraction (to determine carbon content)

xii.	Coarse fraction (to determine carbon content)

xiii.	Root/stick weight (to determine carbon content)

c.	Laboratory data: The soil condition data will be recorded as described above, whereas the mycorrhizae RNA data will generated with Illumina using the methods and metadata methods as described by the Earth Microbiome Project: https://github.com/biocore/emp/blob/master/methods/methods_release1.md
By emulating their management protocol the samples and sequences will be produced generally as follows:

i.	10 individual aliquots samples will be made for each sample with this barcoding system:  Patty_location_plotnumber_a01

ii.	The label will be affixed to the test tubes, and entered into an Excel inventory spread sheet. 

iii.	Metadata curation will follow EML standards, as described: https://github.com/ropensci/EML and set up prior to amplification and sequencing such that the results (the resident species) will be matched with the identifying metadata (type, geographic origin, etc.). This EML file will be created in Rmarkdown.

iv.	The sequencing protocol will follow: https://earthmicrobiome.org/protocols-and-standards/18s/ without a mammal sequence block. The data type produced will be raw FASTQ files

2)	A metadata example similar to what I might generate follows the EML protocol. Seerangan, K., & Thangavelu, M. (2014). Arbuscular mycorrhizal and dark septate endophyte fungal associations in south Indian aquatic and wetland macrophytes. Journal of Botany, 2014. https://doi.org/10.1155/2014/173125 and the dataset/metadata may be found here: doi:10.6073/pasta/b331efa1734c5793978dbe844b981349. 

## Storage and Security

## Access and Data Sharing

a.	The soil nutrient data generated will be shared in plain text formats such as .txt and .csv on GitHub such that Clean Water Services may monitor the research progress. A working metadata “.README” will accompany the uploaded data.

b.	The DNA/RNA data will be shared if the analysis and sharing of these large data files are financially viable. 

c.	All published data sets will carry Creative Commons By Attribution (CCBY; https://creativecommons.org/licenses/by/4.0/)

## Sharing limitations

As the restoration locations are the property of Clean Water Services, public access to the exact restoration locations (GPS coordinates) will be limited to their sharing discretion. Locations will be referred to with individual, unique nomenclature when shared along with a generalized location based upon the Tualatin River’s hydrological units: 17090010.

## Archiving and Preservation

a.	Once the data is finalized, it will be shared in the ScholarsArchive@OSU  at the moment of publication or 2 years after data creation, whichever comes sooner. ScholarsArchive@OSU is committed to long-term accessibility and preservation of research data. 

b.	Physical data sheets will be uploaded digitally and achieved as PDF/A’s with ScholarsArchive@OSU. The physical sheets will be filed and permanently stored with Clean Water Services. 

c.	The physical soil samples will be cataloged and stored securely after final analysis with Clean Water Services.

d.	The physical mycorrhizal RNA/DNA samples will be stored using preservation techniques instructed by the Decomposition Lab until their analysis. After analysis, the generated sequences will be temporarily stored in the Forestry:Groups server, uploaded to ScholarsArchive@OSU, and backed onto a physical hard drive. This data will then be shared to a Clean Water Services server. This will ensure redundancy of these large datafiles.

e.	These data will remain secure and stored at stable conditions as long as support exists at Clean Water Services. 
