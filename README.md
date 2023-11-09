# CHOKE2.0

Data and code accompany Stellpflug, S., Dalrymple, K.A., Stone, D., Southgate, S., Bachman, D., LeFevere, R., Hasan, J., & Zwank, M.D. (under review). Impact Of Repeated Vascular Neck Compression (Sportive Chokes) On Carotid Intima Media Thickness And Brain Injury Biomarkers In Grappling Athletes.

CHOKE 2.0.rmd was programed in 2023.06.0 Build 421 (RStudio Team, 2020), by Kirsten A. Dalrymple, PhD, CCRC.

CHOKE folder contains:
• /CHOKE 2.0.rmd
• /Data_In
• /Data_Out
• /Figures
• /READ ME

FILE AND FOLDER DESCRIPTIONS

/CHOKE 2.0.rmd code to be run in R Studio.

/Data_In:

File name (.csv) and variables 
CHOKE2_Brain
- record_id: subject ID assigned at enrollment
- group: 0 = control, 1 = grappler
- grouptraumahx: 0 = no trauma, 1 = trauma
- nfl: Neurofilament light chain in pg/ml
- hgfap: glial fibrillary acidic protein in pg/ml
- tau: Total Tau in pg/ml
- l1: Upiqui􀆟n C-terminal hydrolase L1 in pg/ml

CHOKE2_CIMT
- record_id: subject ID assigned at enrollment
- group: 0 = control, 1 = grappler
- grouptraumahx: 0 = no trauma, 1 = trauma
- physician: performed ultrasound, coded A, B, C, or D
- cimt_left_lat_1: first left CIMT measurement in mm
- cimt_left_lat_2: second left CIMT measurement in mm
- cimt_left_lat_3: third left CIMT measurement in mm
- cimt_right_lat_1: first right CIMT measurement in mm
- cimt_right_lat_2: second right CIMT measurement in mm
- cimt_right_lat_3: third right CIMT measurement in mm

CHOKE2_CIMTvNorm
- record_id: subject ID assigned at enrollment
- group: 0 = control, 1 = grappler
- grouptraumahx: 0 = no trauma, 1 = trauma
- physician: performed ultrasound, coded A, B, C, or D
- age: participant age at time of ultrasound (years)
- cimt_left_lat_1: first left CIMT measurement in mm
- cimt_left_lat_2: second left CIMT measurement in mm
- cimt_left_lat_3: third left CIMT measurement in mm
- cimt_right_lat_1: first right CIMT measurement in mm
- cimt_right_lat_2: second right CIMT measurement in mm
- cimt_right_lat_3: third right CIMT measurement in mm
- cimt_left: average of three left CIMT measurements in mm
- cimt_right: average of three right CIMT measurements in mm
- predicted_cimt: (0.249 + 0.008*age) from Toseto, et al. (2005)
- left_vs_norm: cimt_left – predicted_cimt
- right_vs_norm: cimt_right – predicted_cimt

CHOKE2_Demographics
- record_id: subject ID assigned at enrollment
- group: 0 = control, 1 = grappler
- grouptraumahx: 0 = no trauma, 1 = trauma
- bloodpressure: 0 = no high blood pressure, 1 = high blood pressure
- tobacco_ever: 0 = never smoked, 1 = smoked
- diabetes: 0 = no diabetes, 1 = diabetes
- cholesterol: 0 = normal cholesterol, 1 = high cholesterol
- stenosis_dissec􀆟on: 0 = no stenosis, 1 = stenosis
- height: height in inches
- weight: weight in lbs.

CHOKE2_PreParticipation
- record_id: subject ID assigned at enrollment
- group: 0 = control, 1 = grappler
- grouptraumahx: 0 = no trauma, 1 = trauma
- age: participant age at time of ultrasound (years)
- gender: 1 = male, 2 = female
- concussion: 0 = no concussion in past 30 days, 1 = concussion in past 30 days
- tbi: 0 = no TBI in past 30 days, 1 = TBI in past 30 days
- symptoms: 0 = no symptoms of TBI or stroke, 1 = symptoms of TBI or stroke
- ever_choked: 0 = never choked, 1 = experienced a choke at some point

CHOKE2_Sport
- record_id: subject ID assigned at enrollment
- group: 0 = control, 1 = grappler
- grouptraumahx: 0 = no trauma, 1 = trauma
- years_grappling: 0 = < 5 years, 1 = 5+ years
- number_chokes: 0 = < 500 chokes, 1 = > 500 chokes
- regular_grappling: 0 = no, 1 = yes
- frequency_athletics: days per week
- primary_athletics: primary sport, freeform
  
/Data_Out: Summary files produced by R code are saved here.

/Figures: Figures produced by R code are saved here.

REFERENCES

RStudio Team (2020). RStudio: Integrated Development for R. RStudio, PBC, Boston, MA URL htp://www.rstudio.com/.

Toseto A, Prati P, Baracchini C, Manara R, Rodeghiero F. Age-adjusted reference limits for carotid intima-media thickness as beter indicator of vascular risk: populatin-based estimates from the VITA project. J Thromb Haemost. 2005;3:1224–1230.
