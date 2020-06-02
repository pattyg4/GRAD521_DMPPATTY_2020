# Data Management Plan

## Data Description

•	Physical samples: These samples will be collected pre and post restoration treatment and will include soil and root samples. The soil samples will have a bulked soil component, a cold stored component to determine mycorrhizal populations, and an archival portion to reference later. Each sample will be save based on a site name, restoration year, date, and numerical system designed to numerate each plot of the study area.

•	Field observations: Pre and post-restoration the GPS location, elevation, soil series evaluation, parent material, soil/air temperatures, and humidity will be documented for each plot. These data will be documented on hard copy data sheet, which will be digitalized as PDF/As. They will then be complied for examination after the data gathering phase. 

•	Laboratory data: A combination of hard copy and digital data sets will record the soil laboratory analysis outputs, which will include mass, nutrient content (nitrogen, phosphorus, potassium, sulfur, and carbon content). The mycorrhizal samples from the soil and roots will have the amplified DNA sequence of the 18S gene (the typical gene sequence for fungi). They will be complied and compared to the datasets existing in the “Basic Local Alignment Search Tool (BLAST)” from the National Center for Biotechnology Information to determine the mycorrhizal populations for each plot and root association. 

For each data type the amount of data generated will be as follows:

a.	Physical samples: 50 MB

b.	Field observations: 50 MB

c.	Laboratory data: upwards of 1 TB depending on how many mycorrhizal DNA sequences are present. 

## Roles and Responsibilities
•	The final responsibility for data management, which includes DMP implementation, data organization, quality control, metadata generation, and data archiving rests with the Master’s student, G. Patty. Patty is also responsible for data dissemination once the final products are produced.

•	Data collection is the primary responsibility of Patty, but additional data collection help and research area maintenance will be shared with the senior field manager of Clean Water Services (CWS), J. Goetz, and possible field technicians.

•	Laboratory analysis and instrument maintenance will be the primary responsibility of Patty, with additional direction from Hatten Soils Lab manager I and the Biodeterioration Lab Senior Faculty Research Assistant. Patty will receive help with the soil samples determining the bulked soil mass in the Hatten lab. In the Biodeterioration Lab, mycorrhizal samples will be processed for DNA sequencing. The nutrient content of the processed and bulked samples will be submitted to OSU’s department of Agriculture, per the recommendation from the Hatten Lab. 

•	Data and statistical analysis is the responsibility of Patty, but direction will be provided by the College of Forestry’s statistician. 

•	If someone were to leave the project, the research would fall upon the senior field manager for CWS, as they own the land and they are funding the research. This may also mean the research becomes proprietary data for Clean Water Services unless they find another graduate student. 

•	There are no data sharing requirements, non-disclosure agreements, nor sensitive and confidential data generate by this project. The goals of this projects are increase the scope and success of restoration by sharing the results with anyone engaged in restoration, both for profit and non-profit groups.


## Data Standards and Metadata

As described in the “Data Description” portion of the DMP, I will generate three types of data: physical samples, field observations, laboratory data.

1.	Physical samples: the physical soil samples will be created in the field for later evaluation in the lab. There will be four sample types,  two for soil condition evaluation, and two for mycorrhizal DNA 18S sequencing. The samples will be titled as follows, first for pre-restoration, then post:

a.	Patty_Pre_sitelocation_plotnumber_datecollected(yyyy/mm/dd)

b.	Patty_Pre_mycor_sitelocation_plotnumber_datecollected(yyyy/mm/dd

c.	Patty_Post_sitelocation_plotnumber_datecollected(yyyy/mm/dd)

d.	Patty_Post_mycor_sitelocation_plotnumber_datecollected(yyyy/mm/dd)

2.	Field and soil condition observations: These observations will be recorded tabularly on site to then be digitized into Excel to match the soil condition file names above. Data “h” through “k” will be recorded in lab and added to the digitized sheets.  

a.	Restoration level (pre or post)

b.	Location: GPS coordinates

c.	Elevation

d.	Vegetation

e.	Soil Temperature

f.	Soil humidity

g.	Soil type

h.	Soil texture

i.	Soil nutrients: nitrogen, phosphorus, potassium, sulfur, and carbon

j.	Bulk density = dry weight/volume (to determine compaction)

k.	Fine fraction (to determine carbon content)

l.	Coarse fraction (to determine carbon content)

m.	Root/stick weight (to determine carbon content)

3.	Laboratory data: The soil condition data will be recorded as described above, whereas the mycorrhizae DNA data will generated with Illumina using the methods and metadata methods as described by the Earth Microbiome Project: https://github.com/biocore/emp/blob/master/methods/methods_release1.md

4.	By emulating their management protocol the samples and sequences will be produced generally as follows:

a.	10 individual aliquots samples will be made for each sample with this barcoding system: 

Patty_ yyyy/mm/dd _location_plotnumber_a01 

b.	The label will be affixed to the test tubes, and entered into an Excel inventory spread sheet. 

c.	Metadata curation will follow EML standards, as described: https://github.com/ropensci/EML and set up prior to amplification and sequencing such that the results (the resident species) will be matched with the identifying metadata (type, geographic origin, etc.). This EML file will be created in Rmarkdown.

d.	The sequencing protocol will follow: https://earthmicrobiome.org/protocols-and-standards/18s/ without a mammal sequence block. The data type produced will be raw FASTQ files.

e.	A metadata example similar to what I might generate follows the EML protocol. Seerangan, K., & Thangavelu, M. (2014). Arbuscular mycorrhizal and dark septate endophyte fungal associations in south Indian aquatic and wetland macrophytes. Journal of Botany, 2014. https://doi.org/10.1155/2014/173125 and the dataset/metadata may be found here: doi.org/10.6073/pasta/b331efa1734c5793978dbe844b981349 


## Storage and Security

1.	The digital data (the raw and edited datasets), except for the DNA sequences, will be stored in six locations, but creating five long term copies: in my personal computer, on the Forestry:Groups sever, in the Box (my OSU account, which will expire after graduation) and Dropbox (my personal account) cloud systems, and backed up on a hard drive to provide to CWS. The DNA sequences will be stored in a FASTQ format on an external hard drive CWS has access to and GitHub if it is financially viable. All these data will also be archived in the ScholarsArchive@OSU to ensure long-term access as well. 

2.	The physical data sample, both the experimental and archival will be cataloged and stored in an on-site facility at CWS. The physical data will exist as long as CWS operates.


## Access and Data Sharing

a.	The soil nutrient data generated will be shared in plain text formats such as .txt and .csv on GitHub such that CWS may monitor the research progress. A working metadata “.README” will accompany the uploaded data.

b.	The DNA data will be shared on GitHub if the analysis and sharing of these large data files are financially viable. 

c.	All published data sets will carry Creative Commons By Attribution (CCBY; https://creativecommons.org/licenses/by/4.0/)


## Sharing limitations

As the restoration locations are the property of Clean Water Services, public access to the exact restoration locations (GPS coordinates) will be limited to their sharing discretion. Locations will be referred to with individual, unique nomenclature when shared along with a generalized location based upon the Tualatin River’s hydrological units: 17090010.

## Archiving and Preservation

a.	Once the data is finalized, it will be shared in the ScholarsArchive@OSU  at the moment of publication or 2 years after data creation, whichever comes sooner. ScholarsArchive@OSU is committed to long-term accessibility and preservation of research data. 

b.	Physical data sheets will be uploaded digitally and achieved as PDF/A’s with ScholarsArchive@OSU. The physical sheets will be filed and permanently stored with CWS. 

c.	The physical soil samples will be cataloged and stored securely after final analysis with CWS.

d.	The physical mycorrhizal DNA samples will be stored using preservation techniques instructed by the Decomposition Lab until their analysis. After analysis, the generated sequences will be temporarily stored in the Forestry:Groups server, uploaded to ScholarsArchive@OSU, and backed onto a physical hard drive. This data will then be shared to a CWS server. This will ensure redundancy of these large datafiles.

e.	These data will remain secure and stored at stable conditions as long as support exists at CWS. 
 
