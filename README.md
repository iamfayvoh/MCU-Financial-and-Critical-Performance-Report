# MCU-Financial-and-Critical-Performance-Report
An executive dashboard analyzing the financial return and critical reception of the Marvel Cinematic Universe. It contrasts production costs against global box office grosses and maps audience versus critic scores to identify the most successful projects across the franchise's phased release strategy.

# Project Overview.
The Marvel Cinematic Universe (MCU) has produced dozens of movies and TV shows across different phases. This project analyzes the financial performance, audience reception, and critic ratings of MCU releases from Phase 1 to Phase 6.

The goal is to understand.
- Which MCU phases performed best financially
- How much profit MCU movies generated
- Which movies had the highest ROI
- How critics and audiences rated MCU releases
- Whether financial performance and audience/critic ratings changed over time

The project was completed using Microsoft Excel, Power Query, PivotTables, and dashboard visualizations.

# Dataset Overview.
The dataset contains 62 MCU releases:
- 38 Movies
- 24 TV Shows
- 6 MCU Phases

Main Data Fields:
- movie_title: Name of the movie or TV show
- mcu_phase: MCU Phase 1–6
- release_date: Release or premiere date
- tomato_meter: Rotten Tomatoes critic score
- audience_score: Rotten Tomatoes audience score
- movie_duration: Movie runtime in minutes
- production_budget: Estimated production cost
- opening_weekend: Domestic opening weekend revenue
- domestic_box_office: Total domestic box office revenue
- worldwide_box_office: Total worldwide box office revenue
- net_profit: Worldwide box office minus production budget
- roi: Return on investment
- movie_type: Movie or TV Show

# Data Cleaning

Before analyzing the data, several cleaning and preparation steps were performed.

Key steps included:

- Converted the dataset into an Excel structured table
- The data was visually analyzed and data issues were spotted and noted.
- I corrected data types and financial formatting for all financial coulumns
- Checked that release dates were properly recognized by excel using the ISNUMBER()
- Further cleaning was done using Power Query
- Cleaned text columns using Power Query by selecting columns then using trim and clean from the format options
- Handled missing values, by changing “NA” cells to “null” to avoid error in power query
- Three helper columns were created to help calculate Net Profit, return on investment and also group the movies with revenue (Movie) from those without revenue (Tv Show) values(movie_type column)

# Calculations

Net Profit = "Worldwide Box Office” - “Production Budget"

ROI = "Net Profit” ÷ “Production Budget"

Note: ROI and profit calculations were only applied to movies because TV shows do not have traditional box-office revenue.»

