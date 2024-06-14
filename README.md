# Prodigy InfoTech Data Science Internship - Task 05

## Task Description
This repository contains the code and documentation for Task 5 completed during my internship at Prodigy Infotech as a Data Science Intern. The task focused on analyzing traffic accident data to identify patterns related to road conditions, weather, and time of day, with the aim of visualizing accident hotspots and contributing factors.

## Data Handling
### Initial Data Overview
The dataset contains over 4.2 million entries and numerous columns, including features such as location (latitude and longitude), weather conditions, road conditions, and time of accidents.

### Data Cleaning
1. **Missing Values**: 
   - Several columns had missing values, which were handled by dropping the columns with the highest percentage of missing data (`End_Lng`, `End_Lat`) and the rows with missing values in other relevant columns (`Visibility(mi)`, `Weather_Condition`, `Humidity(%)`, `Temperature(F)`, `Wind_Direction`, `Pressure(in)`, `Weather_Timestamp`, `Airport_Code`, `Timezone`, `Zipcode`, `Sunrise_Sunset`, `Civil_Twilight`, `Nautical_Twilight`, `Astronomical_Twilight`, `City`, `Description`).

2. **Dropping Columns**: 
   - Dropped the `ID` column as it was not necessary for the analysis.

## Exploratory Data Analysis
### Location Analysis
1. **Accidents by State**: 
   - Visualized the number of accidents per state using a choropleth map of the USA.
   - California (CA) had the highest number of accidents, likely due to its large population.

2. **Accidents by City**: 
   - Plotted the top 50 cities with the highest number of accidents using a bar plot.

3. **Geographical Distribution**: 
   - Created a joint plot of latitude and longitude to visualize the geographical distribution of accidents.

### Weather Conditions
- Analyzed the top 5 weather conditions leading to accidents, with clear weather being the most common condition during accidents.

### Severity Analysis
1. **Severity Distribution**: 
   - Used a bar plot to show the distribution of accident severity levels.
   
2. **Severity by State and City**: 
   - Created bar plots to show the states and cities with the highest severity levels.

### Road and Environmental Conditions
1. **Impact of Road Conditions**: 
   - Analyzed various road conditions and their impact on accidents using pie charts for factors such as the presence of amenities, bumps, crossings, give ways, junctions, no exits, railways, roundabouts, stations, stops, traffic calming measures, and traffic signals.

## Visualizations
### Key Visualizations
- **Choropleth Map**: Number of accidents per state.
- **Bar Plots**: 
  - Top 50 cities with the highest number of accidents.
  - Top 5 weather conditions for accidents.
  - Severity levels of accidents.
  - States and cities with the highest severity levels.
- **Joint Plot**: Geographical distribution of accidents.
- **Pie Charts**: Distribution of various road conditions and their impact on accidents.

## Usage
To reproduce the analysis:
1. Ensure all required libraries are installed (`pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `missingno`).
2. Clone the repository to your local machine.
3. Load the dataset (`US_Accidents_March23.csv`) into a pandas DataFrame.
4. Run the provided Python code in a Jupyter notebook or a Python script.

## Contributions
Contributions to this repository are welcome. Feel free to suggest improvements, report issues, or contribute code to enhance the analysis and visualization process.

## License
This project is licensed under the MIT License.
```
