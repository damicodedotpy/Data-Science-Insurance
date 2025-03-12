<h1>Disclaimer</h1>
<p>
This notebook analyzes a single database containing information about insurance clients and claims. This is a public database sourced from the internet and its data or insights does not represent official insurance results that can be used in real-life applications. However, the following hypotheses and processes are carefully planned and coded to offer a high-quality data science work.
</p>

<h1>Introduction</h1>
<p>The purpose of this data science project is to develop an algorithm capable of predicting loss and froud claims based on clients information.</p>
<p>We also aim to uncover additional insights throughout the project that could be valuable to the insurance industry.</p>

<h1>Dataset Description</h1>
<p>The dataset used for analysis consists of 1000 individual claims, with the primary goal to present Insurance and incident information. The dataset includes 40 different attributes that describe each claim, categorized into four main categories: the insured person, their policy details, incident description, and characteristics of the involved car.</p>

<h1>Columns Description</h1>

* months_as_customer: Number of months the person has been a customer with the insurance company
* age: Age of the insured person
* policy_number: Unique identifier for each insurance policy
* policy_bind_date: Date when the policy was bound
* policy_state: State in which the policy was issued
* policy_csl: Coverage limit of the policy in the form of combined single limits
* policy_deductable: Deductible amount specified in the policy
* policy_annual_premium: Annual premium amount for the policy
* umbrella_limit: Coverage limit provided by an umbrella policy
* insured_zip: ZIP code of the insured person
* insured_sex: Gender of the insured person
* insured_education_level: Education level of the insured person
* insured_occupation: Occupation of the insured person
* insured_hobbies: Hobbies of the insured person
* insured_relationship: Relationship of the insured person with the policyholder
* capital-gains: Capital gains associated with the incident
* capital-loss: Capital losses associated with the incident
* incident_date: Date of the incident
* incident_type: Type of incident (e.g., single vehicle collision, multi-vehicle collision)
* collision_type: Type of collision in the incident
* incident_severity: Severity of the incident
* authorities_contacted: Authorities contacted after the incident
* incident_state: State in which the incident occurred
* incident_city: City in which the incident occurred
* incident_location: Location of the incident
* incident_hour_of_the_day: Hour of the day when the incident occurred
* number_of_vehicles_involved: Number of vehicles involved in the incident
* property_damage: Whether property damage occurred during the incident
* bodily_injuries: Number of bodily injuries in the incident
* witnesses: Number of witnesses present during the incident
* police_report_available: Whether a police report is available for the incident
* total_claim_amount: Total claim amount associated with the incident
* injury_claim: Claim amount for injuries
* property_claim: Claim amount for property damage
* vehicle_claim: Claim amount for vehicle damage
* auto_make: Make of the involved vehicle
* auto_model: Model of the involved vehicle
* auto_year: Year of the involved vehicle
* fraud_reported: Whether the claim is reported as fraudulent (1) or not (0)


<h1>Hypotheses</h1>
<ol>
    <li>
        <p>
            Younger clients are more likely to file a fraud claim.
        </p>
    </li>
    <li>
        <p>
            Older auto models are more likely to be involved in accidents.
        </p>
    </li>
    <li>
        <p>
            Clients with less months as customers are more likely to file a fraudulent claim.
        </p>
    </li>
    <li>
        <p>
            If there is not a police report available, the claim is more likely to be fraudulent.
        </p>
    </li>
    <li>
        <p>
            Clients with poor education levels are more likely to file a fraudulent claim.
        </p>
    </li>
</ol>

<h1>Models Purpose</h1>
<ol>
    <li>Fraud detection.</li>
    <li>Loss amount prediction.</li>
    <li>Dangerous client identification.</li>
</ol>

<h1>Research Methodology</h1>
<p>The following outlines the primary steps undertaken in this investigation:</p>
<ol>
    <li>Loading and analyzing the dataset structure.
        <ol>
            <li>Imports</li>
            <li>Functions</li>
            <li>Constants</li>
            <li>Data load</li>
        </ol>
    </li>
    <li>Exploratory Data Analysis (EDA).</li>
        <ol>
            <li>Data cleaning</li>
            <li>Data completion</li>
            <li>Data casting</li>
            <li>EDA insights</li>
        </ol>
    <li>Data preparation
        <ol>
            <li>Encoding data</li>
            <li>Outliers</li>
            <li>Standardizing data</li>
            <li>Principal features recognition</li>
            <li>Splitting data</li>
            <li>Dimensionality reduction</li>
        </ol>
    </li>
    <li>Model development
        <ol>
            <li>Logistic Regression Model
            <li>Decision Tree Model
            <li>Random Forest Model
        </ol>
    </li>
    <li>Evaluation
        <ol>
            <li>Calculating metrics</li>
            <li>Generating charts</li>
            <li>Deriving insights</li>
            <li>Model selection
        </ol>
    </li>
    <li>Making predictions</li>
    <li>Drawing conclusions</li>
</ol>