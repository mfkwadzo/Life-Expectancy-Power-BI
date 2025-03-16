
## LIFE EXPECTANCY ANALYSIS PROJECT

### Overview
This project analyzes factors affecting life expectancy by incorporating previously overlooked variables such as immunization rates and the Human Development Index (HDI). The analysis is based on a mixed effects model and multiple linear regression, utilizing data from 2000 to 2015 for 193 countries. The focus will be on significant health-related factors, including immunization (Hepatitis B, Polio, Diphtheria), mortality rates, economic conditions, and social factors.

### Motivation
Despite numerous studies on life expectancy influenced by demographic variables and income composition, the impact of immunization and HDI has been largely unexamined. Previous research primarily relied on single-year datasets. This project seeks to fill those gaps and provide a comprehensive analysis that can help countries identify key factors influencing life expectancy.

### Project Objectives
-	Analyze trends in global life expectancy from 2000 to 2015.
-	Examine trends in infant mortality and adult mortality rates over the same period.
-	Investigate the impact of diseases like HIV/AIDS on mortality rates.
-	Compare health outcomes between developed and developing countries.
-	Highlight disparities in life expectancy and mortality rates across continents.
-	Explore the relationship between GDP and life expectancy.
-	Study the correlation between years of schooling and life expectancy.
-	Assess how healthcare expenditure affects life expectancy and mortality.

### Data Sources
The project relies on data accuracy, drawing from the following sources:
-	Global Health Observatory (GHO): Health status and related data for all countries, managed by the World Health Organization (WHO).
-	United Nations: Economic data corresponding to health factors
-	To Understand the life expectancy of the countries more on a continent basis. I decided to add continents dataset from Kaggle by Aadarsh Vani on Countries and continent. 

### Data Structure
The dataset contains 22 columns with various attributes related to life expectancy, health metrics, and socio-economic factors across different countries and years. Key columns include:
-	Country: The country of the observation.
-	Year: The year of the observation.
-	Status: "Developed" or "Developing" country classification.
-	Life expectancy: The average life expectancy in years.
-	Adult Mortality: The adult mortality rate (per 1,000 population).
-	infant deaths: Infant mortality count. (Per 1,000 live births)
-	Alcohol: Per capita alcohol consumption (in litres).
-	percentage expenditure: Percentage of government expenditure on health as a percentage of GDP
-	Hepatitis B, Measles, Polio, Diphtheria: Vaccination coverage rates (%).
-	HIV/AIDS: Prevalence rate of HIV/AIDS (%).
-	thinness (two groups): Rates of undernutrition in children and adolescents.
-	Socio-economic indicators: GDP, Population, Schooling, Income composition of resources: Human Development Index in terms of income composition of resources (index ranging from 0 to 1)

### Data Cleaning
Data was cleaned and Transformed with Power Query
-	Missing values: Hepatitis B (553 missing), GDP (448 missing), Population (652 missing), Alcohol (194 missing).  Income Composition and Schooling. Filled the missing values using column averages.
-	Columns like Life expectancy, Adult Mortality, and others have a smaller number of missing values less than 1%. For this column I removed the data since the missing values are insignificant.
-	Formatted the fields appropriately (year column to text data type).
-	 Cleaned the country column, split and trim column for standardization.
-	The Countries were originally 193 in the dataset but came down to 183 after the data was cleaned.


## KEY INSIGHTS

## Overview
 ## Dashboard 
 ![1](https://github.com/user-attachments/assets/30ff0419-2ad7-46f3-90fb-45114ba1181a))

### Global Average Life Expectancy:
-	The global average life expectancy between 2000 and 2015 is 69.22 years.

Life Expectancy by Status (Developed vs. Developing):
-	Developed countries: Average life expectancy is 79.20 years.
-	Developing countries: Average life expectancy is 67.11 years.
-	This shows a notable disparity, with developed countries having higher life expectancies due to better healthcare systems, infrastructure, and living standards.
 Top and Bottom 10 Countries by Average Life Expectancy:
-	Top 10 Countries: Countries like Japan (82.54 years), Sweden, and Iceland have the highest life expectancy, suggesting superior healthcare systems and lifestyles.
-	Bottom 10 Countries: Countries like Sierra Leone (46.11 years), Central African Republic, and Lesotho have the lowest life expectancy, indicating challenges such as poverty, conflict, or inadequate healthcare access.
Average Adult Mortality by Continent:
-	Africa has the highest average adult mortality rate (266.57), reflecting severe health challenges such as infectious diseases (e.g., HIV/AIDS, malaria), lack of healthcare infrastructure, and socio-economic issues.
-	Europe has the lowest average adult mortality rate (97.39), likely due to advanced healthcare systems and higher standards of living.


## Trends Insights
 
### Life Expectancy Trends:
-	The average life expectancy has been increasing steadily from 2000 to 2015, moving from around 66 years to 72 years. This suggests improvements in healthcare, living conditions, and public health initiatives over time.
Infant Deaths:
-	Total infant deaths recorded is 89.03K. The chart for "Infant Death by Status" indicates a significant disparity between developing and developed regions, with developing regions showing much higher infant mortality rates.
 Adult Mortality:
-	Adult mortality shows fluctuations over the years, with a general decline from 2000 to 2015. However, certain years, such as 2004 and 2008, show peaks in adult mortality rates, which could be due to specific events or crises.
 HIV/AIDS Trend:
-	The average prevalence of HIV/AIDS has significantly declined from 2000 to 2015, dropping from around 3% to close to 1%. This suggests successful efforts in combating HIV/AIDS through awareness, prevention, and treatment programs.


## Socio – Economic Factors
 
### Percentage Expenditure by Status:
-	There is a strong link between healthcare expenditure and life expectancy, with developed nations investing significantly more.
-	Higher spending is associated with a higher average life expectancy whiles Lower spending correlates with a lower average life expectancy.
Average GDP by Continent:
-	Continents with higher GDPs tend to have higher life expectancies:
-	Europe has highest GDP and life expectancy (77 years) and Africa has lowest GDP and life expectancy (59 years).
-	North America, South America, Asia, and Oceania fall between these extremes, showing moderate life expectancy levels and GDPs.

 ### Correlation Between Schooling and Life Expectancy:
-	A positive correlation exists between the average years of schooling and life expectancy.
-	Countries with more education tend to have higher life expectancies, emphasizing the importance of education in improving health outcomes.
Correlation Between GDP and Life Expectancy:
-	A positive correlation is observed between GDP and life expectancy.
-	Countries with higher GDPs generally have better health outcomes, as economic prosperity likely enables better healthcare infrastructure, access to medical services, and higher living standards.


## RECOMMENDATIONS
The following recommendations are proposed to enhance global health outcomes based on the analysis of life expectancy and its associated factors.

### Increase Healthcare Investment:
-	Allocate more resources to healthcare to improve life expectancy, focusing on maternal care, disease prevention, and child health programs which could significantly reduce under-five mortality rates and improve global health outcomes.
-	Partnerships with global health organizations can help bridge funding gaps.
-	Developing Countries should focus on improving healthcare systems, addressing infectious diseases, and promoting maternal and child health programs.

### Research and Policy:
-	Analyze the success factors in countries with high life expectancy (like Japan) to replicate best practices in other countries.
-	Developed countries can share technological advancements, healthcare models, and best practices with developing nations through partnerships or international collaborations.
-	Countries with fluctuating adult mortality rates should be studied further to identify causes, whether they are diseases, economic challenges, or other factors.

### Boost Economic Growth:
-	Strengthen economic policies to boost GDP through industrialization, trade, and diversification of industries.
-	Leverage international aid and development loans for infrastructure and healthcare improvements.
Promote Education:
-	Focus on improving access to education for women and children, as higher levels of education are strongly linked to better health outcomes and increased life expectancy.
-	Develop educational programs aimed at boosting school enrollment and completion rates, especially for girls and underserved communities.
-	Introduce health education initiatives in schools to encourage healthy lifestyle habits and raise awareness about available healthcare services.

For Global Health Efforts: Target interventions in countries with the lowest life expectancy and highest mortality rates, particularly in Africa.

By implementing these recommendations, countries can work towards significantly improving life expectancy and overall health outcomes for their populations.
