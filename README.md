# U.S.-Hospital-Customer-Satisfaction-2016-2020-
How satisfied are U.S. patients? Is a hospital's overall score really determined by how well it provides good customer services? Are there types of hospitals or regions where patient satisfaction is better or worse?

Every year, all U.S. hospitals that accept payments from Medicare and Medicaid must submit quality data to The Centers for Medicare and Medicaid Services (CMS). CMS' Hospital Compare program is a consumer-oriented website that provides information on "the quality of care hospitals are providing to their patients." CMS releases this quality data publicly in order to encourage hospitals to improve their quality and to help consumer make better decisions about which providers they visit.

"Hospital Compare provides data on over 4,000 Medicare-certified hospitals, including acute care hospitals, critical access hospitals (CAHs), children’s hospitals, Veterans Health Administration (VHA) Medical Centers, and hospital outpatient departments"

The Centers for Medicare & Medicaid Services (CMS) uses a five-star quality rating system to measure the experiences Medicare beneficiaries have with their health plan and health care system — the Star Rating Program. Health plans are rated on a scale of 1 to 5 stars, with 5 being the highest.

One part of a hospital's overall rating is it's patient satisfaction survey scores. CMS attempts to take into consideration how well patients are treated by the provider. A description of HCAHPS can be found here ***HCAHPS Description.

# Inspiration
Since I work in healthcare, I was inspired to look at my own hospital's performance. Since CMS provides overall performance data on over 4,000 facilities, I hope this data can help people answer the following questions:

Which hospitals have the best overall performance? Best performance by measure such as Patient Experience?
Which states, cities, counties have the most high-performing hospitals? The lowest performing hospitals?
How have individual hospitals overall performance changed between 2016 and 2020? Are certain locations getting better or worse overall?
Is the overall CMS star rating correlated with patient satisfaction?
Can we predict a hospital overall rating from its patient satisfaction scores?
Which survey questions are most informative of a hospital's overall quality?

Filename	Year	Dataset Rows	Dataset Columns
cmshospitalpatientsatisfaction2020.csv	2020	442587	43
cmshospitalpatientsatisfaction2019.csv	2019	442401	43
cmshospitalpatientsatisfaction2018.csv	2018	239650	43
cmshospitalpatientsatisfaction2017.csv	2017	264660	43
cmshospitalpatientsatisfaction2016.csv	2016	264385	43
Includes the most recent Hospital General Information.csv data for each archive year found on CMS' archive site. Years: 2016-2020
NOTE: Some Hospital Medicare IDs have leading zeroes. Be sure to read Facility ID column as a string.
# Dataset columns
Column Name	Data Type	Description
Facility ID	Char(6)	Facility Medicare ID
Facility Name	Char(72)	Name of the facility
Address	Char(51)	Facility street address
City	Char(20)	Facility City
State	Char(2)	Facility State
ZIP Code	Num(8)	Facility ZIP Code
County Name	Char(25)	Facility County
Phone Number	Char(14)	Facility Phone Number
HCAHPS Measure ID	Char(25)	HCAHPS Patient Survey Measure Name
HCAHPS Question	Char(138)	HCAHPS Patient Survey Question
HCAHPS Answer Description	Char(118)	HCAHPS Patient Survey Answer
Patient Survey Star Rating	Char(14)	Overall rating for survey item
Patient Survey Star Rating Footnote	Char(7)	n/a
HCAHPS Answer Percent	Char(14)	Percent of surveys with question answered
HCAHPS Answer Percent Footnote	Char(8)	n/a
HCAHPS Linear Mean Value	Char(14)	HCAHPS Patient Survey question linear mean value
Number of Completed Surveys	Char(13)	Number of completed surveys for hospital. N-size.
Number of Completed Surveys Footnote	Char(8)	n/a
Survey Response Rate Percent	Char(13)	Hospital survey response rate.
Survey Response Rate Percent Footnote	Char(8)	n/a
Start Date	Date	Survey collection period start date
End Date	Date	Survey collection period end date
Year	Char(4)	cms data release year
Hospital Type	Char(34)	What type of facility is it?
Hospital Ownership	Char(43)	What type of ownership does the facility have?
Emergency Services	Char(3))	Does the facility have emergency services Yes/No?
Meets criteria for promoting interoperability of EHRs	Char(1)	Does facility meet government EHR standard Yes/No?
Hospital overall rating	Char(13)	Hospital Overall Star Rating 1=Worst; 5=Best. Aggregate measure of all other measures
Hospital overall rating footnote	Num(8)	
Mortality national comparison	Char(28)	Facility overall performance on mortality measures compared to other facilities
Mortality national comparison footnote	Num(8)	
Safety of care national comparison	Char(28)	Facility overall performance on safety measures compared to other facilities
Safety of care national comparison footnote	Num(8)	
Readmission national comparison	Char(28)	Facility overall performance on readmission measures compared to other facilities
Readmission national comparison footnote	Num(8)	
Patient experience national comparison	Char(28)	Facility overall performance on pat. exp. measures compared to other facilities
Patient experience national comparison footnote	Char(8)	
Effectiveness of care national comparison	Char(28)	Facility overall performance on effect. of care measures compared to other facilities
Effectiveness of care national comparison footnote	Char(8)	
Timeliness of care national comparison	Char(28)	Facility overall performance on timeliness of care measures compared to other facilities
Timeliness of care national comparison footnote	Char(8)	
Efficient use of medical imaging national comparison	Char(28)	Facility overall performance on efficient use measures compared to other facilities
Efficient use of medical imaging national comparison footnote
