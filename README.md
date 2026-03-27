## Business Context
Understanding crime patterns is essential for identifying risk factors, improving public safety strategies, and supporting decision-making in law enforcement and policy design.

## Objective
Analyze the dataset to identify patterns in crime characteristics such as demographics, victim-offender relationships, and incident types.

## Dataset Description
The dataset contains information about crime incidents, including:

- Offender demographics (age, gender, race)
- Victim demographics (age, gender, race)
- Crime category
- Report type
- Fatal vs non-fatal outcomes

## Data Cleaning Process
Several preprocessing steps were required to ensure data quality:

- Standardization of column names (removing spaces and formatting)
- Detection and removal of duplicate records (~30% of the dataset)
- Cleaning of categorical variables (uppercase and trimming text)
- Identification and handling of unrealistic values (e.g., victim age > 100)
- Creation of a clean dataset for analysis

## Feature Engineering
A new variable was created to enhance analysis:

- `age_gap`: Difference between victim age and offender age

This feature allows deeper analysis of relationships between victims and offenders.

## Exploratory Data Analysis (EDA)

The analysis focused on identifying meaningful patterns in the data:

### Age Distribution
- Most observations are concentrated between 20–40 years
- Victims and offenders tend to fall within similar age ranges

### Victim vs Offender Relationship
- No strong relationship between ages
- Crimes occur across a wide range of age combinations

### Crime Category Analysis
- Violence is the most frequent category
- Followed by Theft and Miscellaneous

### Fatal vs Non-Fatal Incidents
- The majority of incidents are non-fatal
- Fatal cases are rare and mostly associated with violent crimes

### Gender Patterns
- Male offenders dominate across all categories
- Indicates a strong gender imbalance in crime participation

### Age Gap Analysis
- Age differences vary depending on the type of crime
- Some crimes involve significant differences between victim and offender ages

### Race Interaction
- Interactions often occur within the same demographic group
- Suggests possible geographic or social clustering

## Key Insights

- Crime patterns are primarily driven by categorical variables rather than numerical ones
- Violence is the dominant category across the dataset
- Most incidents are non-fatal, indicating lower severity in most reported cases
- There is a strong predominance of male offenders
- Age alone does not explain crime dynamics effectively

## Conclusion

The analysis shows that crime patterns are influenced more by demographic and categorical variables than by numerical factors such as age.

The presence of a large number of duplicate records highlights the importance of data cleaning, as failing to address this would have significantly biased the results.

Additionally, the weak relationships between numerical variables suggest that predictive modeling would require careful feature engineering, with a stronger focus on categorical variables.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Project Structure

- `crimen.ipynb` → Data cleaning and analysis
- `README.md` → Project documentation

## Skills Demonstrated
