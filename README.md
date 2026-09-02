# WHO Global Health Statistics Analysis, Exploring the Relationship Between Healthcare Access, Environmental Conditions, and Health Outcomes

## Project Summary
An end-to-end analytical study evaluating global health inequalities using World Health Organization (WHO) health statistics. This project investigates how healthcare access (workforce density, skilled birth attendance, immunisation), environmental conditions (air pollution, clean water, sanitation), and disease burden interact to shape life expectancy, infant and child mortality, and regional health disparities over time.
## Core Guiding Question
How do healthcare access, environmental conditions, and disease burden influence health outcomes and health inequalities across countries and regions over time, specifically, how does life expectancy vary across countries and regions, and what factors are associated with these differences?

## Data Used
[Dataset](https://www.kaggle.com/datasets/utkarshxy/who-worldhealth-statistics-2020-complete)

### 1. Global Health Disparities
<img width="2062" height="1153" alt="KPI Global Health Disparities" src="https://github.com/user-attachments/assets/53302526-d6e5-489d-86b6-f1d30e442403" />


### Questions & Insights

- **Which countries have the highest and lowest life expectancy?**

**Insights**: European and Asian nations (e.g., Japan, Switzerland, Spain, Singapore) top the list near 80–84 years, whereas African nations (e.g., Lesotho, Central African Republic, Eswatini, Somalia) rank lowest near 50–60 years.
- **How do infant, neonatal, and under-5 mortality rates vary across continents/countries?**
  
**Insights**: Africa with 92.52 per 1,000 of children being born, records the highest average child mortality in the dataset, while Europe records the lowest 15.99 per 1,000. This highlights substantial regional inequalities in infant and child survival.
- **What's the global gap between doctor density and basic water access?**

**Insights**: Doctor density averages 20.69/10,000, but basic water access sits at 77.85% access to clean water is far more widespread globally than access to physicians.
- **Which sex shows consistently higher life expectancy?**

**Insights**: The lighter line (female) tracks visibly above the darker line (male) across almost the entire country axis except Qatar.
- **Does maternal mortality look proportionate to infant mortality?**

**Insights**: Yes, maternal mortality sits at 210.31 per 100,000 and infant mortality at 53.81 per 1,000, and both point to the same underlying gap in reproductive/perinatal care access rather than two unrelated problems.
- **How does the adolescent birth rate vary across countries?**

**Insights**: Extremely right skewed; rates hover below 10 per 1,000 in Europe and East Asia, but jump to 100–150+ per 1,000 across parts of Africa and South America. 


### 2. Clinical Workforce & Mortality
<img width="2063" height="1160" alt="Clinical Workforce   Mortality" src="https://github.com/user-attachments/assets/3b2fef61-83ef-4f4d-8035-ad7765f9119d" />


### Questions & Insights

- **Is there a stronger relationship between mortality and nurses/midwives, or mortality and doctors?**

**Insights**: Both show a similar steep inverse exponential curve, but the "nurses & midwives" scatter has a longer tail of high density, low mortality points nursing capacity seems to matter as much as, or more than, doctor supply at the low end
- **Does infant mortality rate differ by gender, and if so, in which direction?**

**Insights**: Based on the scatterplots (Infant Mortality vs. Nursing & Midwifery Density, and vs. Medical Doctors Density), both sexes are plotted, Female (blue) and Male (orange) across the full range of workforce density, and both series follow the same steep downward curve as density increases. The two groups move together rather than diverging, meaning the dominant driver of infant mortality in this data is healthcare workforce access, not gender.
- **At what workforce density does infant mortality flatten out near its minimum?**

**Insights**: Roughly 40–60 nurses/midwives per 10,000, mortality drops below 50 and stays low, a plausible "diminishing returns" threshold.

### 3. Reproductive Care & Risk Factors
<img width="2063" height="1158" alt="Reproductive Care   Risk Factors" src="https://github.com/user-attachments/assets/6fe89ac4-79d8-4d75-b80e-c2732aa95df2" />


### Questions & Insights

- **Does higher skilled birth attendance actually reduce maternal mortality here?**

**Insights**: Yes the scatter is a clean downward curve; countries above ~80% skilled attendance cluster near the bottom of the mortality axis.
- **Is alcohol consumption a strong predictor of suicide rate?**

**Insights**: Weakly  there's a general upward drift, but the spread is wide (e.g., points at 5L consumption range from ~5 to ~35 suicides/100k), so other factors clearly dominate.
- **How does adolescent birth rate relate to maternal mortality?**

**Insights**: Positively and fairly strongly high adolescent birth rate countries also show the highest maternal mortality outliers (1000+) which is of sierra leone.


### 4. Environmental Determinants & Disease Burden
<img width="2055" height="1150" alt="Environmental Determinants   Disease Burden" src="https://github.com/user-attachments/assets/862a4c5b-9e6a-46b0-b082-66210c742d5c" />


### Questions & Insights

- **How does the air pollution death rate relate to life expectancy across countries?**

**Insights**: The scattered chart demonstrates a clear negative correlation: countries with higher air pollution death rates (exceeding 60–80 per 100,000) 2. cluster at significantly lower life expectancies (<65 years).
- **Which environmental factor tracks life expectancy most tightly: water access, sanitation, or clean fuel?**

**Insights**: All three show similar positive linear trends; sanitation and water access scatters look marginally tighter (less vertical spread) than clean fuel. 
- **Which disease category drives the most air pollution deaths, and where?**

**Insights**: Ischaemic heart disease and lower respiratory infections dominate the treemap, both concentrated heavily in Asia, Oceania and Africa.
- **Does air pollution death rate cleanly predict life expectancy?**

**Insights**: Inversely, yes  but with real scatter (some regions have moderate pollution and still high life expectancy), suggesting confounding by income/healthcare access.

### 5. Disease Burden & Health Risk Factors
<img width="2065" height="1160" alt="Disease Burden   Health Risk Factors" src="https://github.com/user-attachments/assets/b431dddb-6f24-4470-b956-c357f054e192" />


### Questions & Answers

- **How do TB, malaria, and new HIV infection rates differ across countries and regions?**

**Insights**: African regions carry the heavy majority of Malaria incidence and new HIV infections, whereas TB incidence remains broadly elevated across both African and Asian regions. 
- **How does Hepatitis B surface antigen prevalence vary across countries?**

**Insights**: Highest among young children in the African region (>3% prevalence), compared to <1% in European and Americas regions due to universal infant vaccination. 
- **Which continent has cut tobacco use the most?**

**Insights**: Oceania starts highest (~38%) and Europe follows, while North America ends lowest (~20%)  the line is monotonically declining across all continents shown.
- **Which countries carry the highest combined burden of malaria, TB, and HIV?**

**Insights**: African countries. 
- **Where does new HIV incidence concentrate?**

**Insights**: Africa dominates sharply (~2.2/1,000) with a steep drop-off; every other continent sits under 0.5.
- **Which countries/regions achieved the steepest decline in premature mortality from CVD, cancer, diabetes, and chronic respiratory disease (ages 30–70), and what factors (healthcare access, tobacco use) track alongside it?**

**Insights**: Europe achieved the steepest declines in 30–70 CVD mortality, driven by robust primary healthcare access, early screening, and aggressive anti tobacco legislation. 
- **Is CVD mortality risk inversely related to infectious disease burden by continent?**

**Insights**: Partially Oceania/Africa show higher NCD risk despite Africa also carrying the HIV burden, meaning some regions face a double burden rather than a clean trade-off.

### 6. Health Risk Factors & NCD Outcomes 
<img width="2065" height="1156" alt="HealthEnviroment Risk Factors   NCD Outcomes" src="https://github.com/user-attachments/assets/21abe6c9-fc02-45b3-beca-120a9c09a495" />


### Questions & Answers

- **Is the reported number of people requiring interventions against NTDs associated with life expectancy?**

**Insights**: No clear relationship is visible. Most locations cluster near very low reported NTD intervention needs while life expectancy varies considerably. There is also a major high value outlier, but its life expectancy is not unusually low, so the chart does not support a strong relationship between reported NTD burden and life expectancy.
- **Is tobacco use prevalence associated with premature NCD mortality?**

**Insights**:Countries with higher tobacco use prevalence generally show higher premature NCD mortality risk, although substantial variation exists. This suggests tobacco use is an important risk factor, but it does not fully explain differences in premature NCD mortality across countries. 
- **Which countries report the highest and lowest prevalence of intimate partner violence against women?**

**Insights**: Equatorial Guinea reports the highest at roughly 45%+, with Afghanistan, Vanuatu, and Kiribati close behind in the high 30s to lown 40s. Prevalence declines gradually and continuously across the ~90 countries shown, down to under 5% for the lowest reporters (Lithuania, Malta, and several others cluster at the bottom). High prevalence countries span multiple regions, Africa, Pacific Islands, and Asia all appear near the top rather than being confined to one geography. 



## CONCLUSION
This analysis set out to understand how healthcare access, environmental conditions, and disease burden are associated with global health outcomes. Across the dataset, the clearest and most consistent pattern is that structural access including healthcare workforce density, skilled birth attendance, and access to basic water, sanitation, and fuel tracks closely with life expectancy and mortality outcomes, more consistently than behavioral factors such as alcohol or tobacco use, whose relationships with health outcomes were present but more variable. Africa recurs throughout the analysis as a region facing a compounding health burden, characterized by lower workforce density, higher infectious disease incidence, and substantial NCD burden simultaneously rather than a single isolated challenge.
Not every hypothesized relationship held up under inspection. Reported NTD intervention needs showed no discernible relationship with life expectancy, underscoring that raw burden counts do not necessarily reflect treatment effectiveness or quality of care. Tobacco prevalence showed only a weak to moderate association with premature NCD mortality rather than the strong relationship often assumed, suggesting that tobacco use is one contributing risk factor among several rather than a dominant factor on its own.

## LIMITATIONS
* **Sparse and irregular time coverage:**

The Year field contains sparse and irregular reporting points rather than continuous annual observations across the full 1920–2018 range. Because large gaps exist between some reporting years, conventional continuous trend charts could imply changes that are not directly supported by observed data. A reliable change over time analysis would therefore require either restricting the analysis to periods with sufficient reporting coverage or presenting sparse observations as discrete data points rather than as a continuous trend.

* **Incomplete indicator and country coverage:**

Data availability varies considerably across indicators and countries. Indicators such as gender based violence have substantial missingness, which limits the reliability of some country and regional comparisons. Apparent differences may therefore partly reflect variations in reporting coverage rather than differences in the underlying health conditions.

* **Cross-sectional associations rather than causation:**

Most of the relationships examined are based on comparisons between countries rather than consistent longitudinal observations. Therefore, the analysis identifies associations but cannot establish that one factor directly causes a change in another. For example, an association between higher healthcare workforce density and lower mortality does not by itself demonstrate that greater workforce density caused the lower mortality.

* **Overall data coverage:**

The dataset has an overall data collection coverage of approximately 63.32%, meaning that a substantial proportion of the expected observations are unavailable. This incomplete coverage may introduce gaps in country level and indicator level comparisons and may limit the generalizability of some findings.

* **Potential confounding factors:**

Life expectancy and mortality are influenced by many factors not included in this analysis, including socioeconomic conditions, education, nutrition, demographics, government policy, and broader healthcare system characteristics. These factors may contribute to the relationships observed between healthcare access, environmental conditions, disease burden, and health outcomes.

* **Derived regional classification:**

The source data did not provide a consistent regional grouping across the indicators. A DAX based country-to-continent classification was therefore created for regional analysis. While necessary for consistent regional comparisons within the dashboard, this classification is a derived modeling field rather than an original variable supplied by the source dataset.

***Outliers and data comparability:**

Some indicators contain extreme observations, while reporting coverage and measurement practices may vary across countries. Outliers were not automatically removed because an unusual observation is not necessarily erroneous or invalid. However, extreme values can influence observed relationships and should therefore be interpreted alongside the broader distribution of the data. Differences in reporting methodology and coverage may also affect cross country comparisons.

## ROUND-UP
Overall, the findings suggest that access related factors are among the factors most consistently associated with better health outcomes in this dataset. Healthcare workforce capacity and essential infrastructure therefore emerge as important areas for further investigation, while recognizing that these relationships are associative rather than causal.
Beyond the broader patterns, several countries and regions stand out on the access indicators examined. Countries with high skilled birth attendance, workforce density, and WASH coverage particularly across Europe, parts of Asia, and North America tend to show a more favorable combination of lower maternal and infant mortality and stronger basic services access. Conversely, countries with lower performance across these access indicators, particularly in parts of Africa, experience some of the highest combined burdens across the access related measures examined.
These comparisons describe relative performance on the selected health access indicators only and should not be interpreted as a broader assessment of quality of life, safety, cost of living, or suitability for relocation, which fall outside the scope of this dataset.
