# Amini-Assignment
Health Registry Data Cleaning and Exploratory Data Analysis Assignment. 

<h1>Overview</h1>  

This notebook performs exploratory data analysis (EDA) and cleaning on a healthcare facilities registry dataset. The dataset contains information about various healthcare facilities including facility IDs, names, types, capacities, regions, licensing dates, inspection dates, GPS locations, and remarks. This was done with limited time. 

<h1>Key Steps Performed</h1>
<ol>
1. Initial Data Inspection
Identified dataset structure (9 columns, 13,013 entries)

Analyzed missing values:

facility_id: 3,708 missing

facility_type: 1,998 missing

capacity: 2,652 missing

gps_location: 2,292 missing

Found and removed 1,672 duplicate rows

2. Data Cleaning
facility_id: Removed special characters, filled missing values with "missing"

facility_name: Removed parentheses content, emojis, and special characters

facility_type:

Standardized values (e.g., "Health Ctr." → "health center")

Mapped to consistent categories (hospital, clinic, etc.)

region:

Fixed backwards names (e.g., "werdna .ts" → "st. andrew")

Standardized using fuzzy matching with parish names

capacity:

Converted text numbers to digits (e.g., "ten beds" → 10)

Extracted numerical values

gps_location:

Split into latitude and longitude columns

Converted various formats to decimal coordinates

dates: Converted to datetime format

remarks: Cleaned text and standardized case

<li>EDA Findings</li>
Capacity Analysis (by facility type):

Clinic: 146 avg capacity

Community Health Center: 152

Health Center: 136

Hospital: 147

Polyclinic: 144

Regional Distribution: Standardized 11 parishes including "st. andrew", "st. george", "christ church", etc.

GPS Coordinates: Cleaned and extracted valid latitude/longitude pairs

<li>4. Output </li>
Key Steps Performed
1. Initial Data Inspection
Identified dataset structure (9 columns, 13,013 entries)

Analyzed missing values:

facility_id: 3,708 missing

facility_type: 1,998 missing

capacity: 2,652 missing

gps_location: 2,292 missing

Found and removed 1,672 duplicate rows

2. Data Cleaning
facility_id: Removed special characters, filled missing values with "missing"

facility_name: Removed parentheses content, emojis, and special characters

facility_type:

Standardized values (e.g., "Health Ctr." → "health center")

Mapped to consistent categories (hospital, clinic, etc.)

region:

Fixed backwards names (e.g., "werdna .ts" → "st. andrew")

Standardized using fuzzy matching with parish names

capacity:

Converted text numbers to digits (e.g., "ten beds" → 10)

Extracted numerical values

gps_location:

Split into latitude and longitude columns

Converted various formats to decimal coordinates

dates: Converted to datetime format

remarks: Cleaned text and standardized case

<li> EDA Findings</li>
Capacity Analysis (by facility type):

Clinic: 146 avg capacity

Community Health Center: 152

Health Center: 136

Hospital: 147

Polyclinic: 144

Regional Distribution: Standardized 11 parishes of Barbados

GPS Coordinates: Cleaned and extracted valid latitude/longitude pairs

4. Output
Cleaned dataset exported to cleaned_health_registry.csv
</ol>
Cleaned dataset exported to cleaned_health_registry.csv
