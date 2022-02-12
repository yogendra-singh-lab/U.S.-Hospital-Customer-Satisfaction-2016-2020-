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


<table>
    <thead>
        <tr>
            <th>Filename</th>
            <th>Year</th>
            <th>Dataset Rows</th>
            <th>Dataset Columns</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>cms<em>hospital</em>patient<em>satisfaction</em>2020.csv</td>
            <td>2020</td>
            <td>442587</td>
            <td>43</td>
        </tr>
        <tr>
            <td>cms<em>hospital</em>patient<em>satisfaction</em>2019.csv</td>
            <td>2019</td>
            <td>442401</td>
            <td>43</td>
        </tr>
        <tr>
            <td>cms<em>hospital</em>patient<em>satisfaction</em>2018.csv</td>
            <td>2018</td>
            <td>239650</td>
            <td>43</td>
        </tr>
        <tr>
            <td>cms<em>hospital</em>patient<em>satisfaction</em>2017.csv</td>
            <td>2017</td>
            <td>264660</td>
            <td>43</td>
        </tr>
        <tr>
            <td>cms<em>hospital</em>patient<em>satisfaction</em>2016.csv</td>
            <td>2016</td>
            <td>264385</td>
            <td>43</td>
        </tr>
    </tbody>
</table>


Includes the most recent Hospital General Information.csv data for each archive year found on CMS' archive site. Years: 2016-2020
NOTE: Some Hospital Medicare IDs have leading zeroes. Be sure to read Facility ID column as a string.

# Dataset columns

<table>
    <thead>
        <tr>
            <th>Column Name</th>
            <th>Data Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Facility ID</td>
            <td>Char(6)</td>
            <td>Facility Medicare ID</td>
        </tr>
        <tr>
            <td>Facility Name</td>
            <td>Char(72)</td>
            <td>Name of the facility</td>
        </tr>
        <tr>
            <td>Address</td>
            <td>Char(51)</td>
            <td>Facility street address</td>
        </tr>
        <tr>
            <td>City</td>
            <td>Char(20)</td>
            <td>Facility City</td>
        </tr>
        <tr>
            <td>State</td>
            <td>Char(2)</td>
            <td>Facility State</td>
        </tr>
        <tr>
            <td>ZIP Code</td>
            <td>Num(8)</td>
            <td>Facility ZIP Code</td>
        </tr>
        <tr>
            <td>County Name</td>
            <td>Char(25)</td>
            <td>Facility County</td>
        </tr>
        <tr>
            <td>Phone Number</td>
            <td>Char(14)</td>
            <td>Facility Phone Number</td>
        </tr>
        <tr>
            <td>HCAHPS Measure ID</td>
            <td>Char(25)</td>
            <td>HCAHPS Patient Survey Measure Name</td>
        </tr>
        <tr>
            <td>HCAHPS Question</td>
            <td>Char(138)</td>
            <td>HCAHPS Patient Survey Question</td>
        </tr>
        <tr>
            <td>HCAHPS Answer Description</td>
            <td>Char(118)</td>
            <td>HCAHPS Patient Survey Answer</td>
        </tr>
        <tr>
            <td>Patient Survey Star Rating</td>
            <td>Char(14)</td>
            <td>Overall rating for survey item</td>
        </tr>
        <tr>
            <td>Patient Survey Star Rating Footnote</td>
            <td>Char(7)</td>
            <td>n/a</td>
        </tr>
        <tr>
            <td>HCAHPS Answer Percent</td>
            <td>Char(14)</td>
            <td>Percent of surveys with question answered</td>
        </tr>
        <tr>
            <td>HCAHPS Answer Percent Footnote</td>
            <td>Char(8)</td>
            <td>n/a</td>
        </tr>
        <tr>
            <td>HCAHPS Linear Mean Value</td>
            <td>Char(14)</td>
            <td>HCAHPS Patient Survey question linear mean value</td>
        </tr>
        <tr>
            <td>Number of Completed Surveys</td>
            <td>Char(13)</td>
            <td>Number of completed surveys for hospital. N-size.</td>
        </tr>
        <tr>
            <td>Number of Completed Surveys Footnote</td>
            <td>Char(8)</td>
            <td>n/a</td>
        </tr>
        <tr>
            <td>Survey Response Rate Percent</td>
            <td>Char(13)</td>
            <td>Hospital survey response rate.</td>
        </tr>
        <tr>
            <td>Survey Response Rate Percent Footnote</td>
            <td>Char(8)</td>
            <td>n/a</td>
        </tr>
        <tr>
            <td>Start Date</td>
            <td>Date</td>
            <td>Survey collection period start date</td>
        </tr>
        <tr>
            <td>End Date</td>
            <td>Date</td>
            <td>Survey collection period end date</td>
        </tr>
        <tr>
            <td>Year</td>
            <td>Char(4)</td>
            <td>cms data release year</td>
        </tr>
        <tr>
            <td>Hospital Type</td>
            <td>Char(34)</td>
            <td>What type of facility is it?</td>
        </tr>
        <tr>
            <td>Hospital Ownership</td>
            <td>Char(43)</td>
            <td>What type of ownership does the facility have?</td>
        </tr>
        <tr>
            <td>Emergency Services</td>
            <td>Char(3))</td>
            <td>Does the facility have emergency services Yes/No?</td>
        </tr>
        <tr>
            <td>Meets criteria for promoting interoperability of EHRs</td>
            <td>Char(1)</td>
            <td>Does facility meet government EHR standard Yes/No?</td>
        </tr>
        <tr>
            <td>Hospital overall rating</td>
            <td>Char(13)</td>
            <td>Hospital Overall Star Rating 1=Worst; 5=Best. Aggregate measure of all other measures</td>
        </tr>
        <tr>
            <td>Hospital overall rating footnote</td>
            <td>Num(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Mortality national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on mortality measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Mortality national comparison footnote</td>
            <td>Num(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Safety of care national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on safety measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Safety of care national comparison footnote</td>
            <td>Num(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Readmission national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on readmission measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Readmission national comparison footnote</td>
            <td>Num(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Patient experience national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on pat. exp. measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Patient experience national comparison footnote</td>
            <td>Char(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Effectiveness of care national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on effect. of care measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Effectiveness of care national comparison footnote</td>
            <td>Char(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Timeliness of care national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on timeliness of care measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Timeliness of care national comparison footnote</td>
            <td>Char(8)</td>
            <td></td>
        </tr>
        <tr>
            <td>Efficient use of medical imaging national comparison</td>
            <td>Char(28)</td>
            <td>Facility overall performance on efficient use measures compared to other facilities</td>
        </tr>
        <tr>
            <td>Efficient use of medical imaging national comparison footnote</td>
            <td>Char(8)</td>
            <td>n/a</td>
        </tr>
    </tbody>
</table>
