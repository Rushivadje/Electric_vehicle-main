# Electric Vehicle Data Analysis
# Overview
  This project provides an in-depth analysis of electric vehicle (EV) data, exploring patterns and trends in vehicle models, types, range, and location-based distributions. The analysis aims to offer insights into the growth of electric vehicles, their geographic spread, and cost factors in the market.

# Motivation
The motivation for this project stemmed from the growing interest in sustainable transportation and the impact of electric vehicles on reducing carbon emissions. By analyzing EV market trends, the goal is to provide insights that can help accelerate the transition to eco-friendly transportation.

# Project Structure
1. Problem Definition

   To analyze electric vehicle data and extract meaningful insights on demographics, vehicle characteristics, and fuel type eligibility to understand the factors affecting the EV market.

3. Dataset Information

   The dataset consists of 130,443 entries with the following 17 columns:

        VIN (1-10): Partial Vehicle Identification Number
        
        County, City, State, Postal Code: Location data for the vehicle
        
        Model Year: Year the vehicle was manufactured
        
        Make and Model: Manufacturer and specific model of the vehicle
        
        Electric Vehicle Type: Type of electric vehicle (e.g., BEV, PHEV)
        
        CAFV Eligibility: Eligibility status for Clean Alternative Fuel Vehicle designation
        
        Electric Range: Range of the vehicle on a full charge (in miles)
        
        Base MSRP: Manufacturer's Suggested Retail Price
        
        Legislative District: Political district of the vehicle’s registration
        
        DOL Vehicle ID: Department of Licensing unique identifier for the vehicle
        
        Vehicle Location: Approximate location information
        
        Electric Utility: Utility provider for the vehicle’s location
        
        2020 Census Tract: Census tract data for demographic analysis

3. Data Cleaning and Preprocessing

        Handled Duplicates: Checked and removed any duplicate entries.

        Dropping Irrelevant Columns: Removed columns such as VIN (1-10), Base MSRP, Legislative District, DOL Vehicle ID, Vehicle Location, and 2020 Census Tract to focus on relevant data.

        Missing Values: Managed missing values in columns like Model, County, City, and Vehicle Location.
        
        Data Type Segmentation: Segregated features into categorical and numerical lists for easier analysis.
        
        Encoding: Encoded categorical variables where necessary.

6. Exploratory Data Analysis (EDA):

    Analyzed various features, including:
    
        Geographic Spread: Visualized distribution of EVs across different states and counties.
        
        Yearly Trends: Analyzed model years to understand the growth trajectory of EVs.
        
        Electric Range and MSRP: Explored how range and pricing affect the EV market and consumer choice.
        
        CAFV Eligibility: Examined the eligibility distribution for clean alternative fuel vehicles.

3. Data Analysis

   Key analyses performed on the dataset:

        Electric Range Insights: Identified the maximum electric range and details of the corresponding vehicle.
        
        CAFV Eligibility and Vehicle Type: Analyzed counts for CAFV eligibility and electric vehicle types.

        Model Year Distribution: This operation gives the frequency of each model year in the dataset. It helps identify the distribution of EVs based on their manufacturing years.
        
        Most Common Model Year: This returns the most frequent model year in the dataset, highlighting the year with the most EV entries.
        
        Top 10 EV Makes: This shows the top 10 most common EV makes in the dataset, offering insights into the most popular manufacturers.
        
        Top 10 Cities with EVs: This lists the top 10 cities with the highest number of EVs, highlighting geographic areas with significant EV adoption.
        
        Top 10 Counties with EVs: This reveals the top 10 counties with the highest number of EVs, which helps us understand regional EV penetration.
        
        Top 15 States with EVs: This operation provides the top 15 states with the highest number of electric vehicles, focusing on state-level trends.
        
        Top 10 EV Models: This shows the top 10 most popular EV models, helping identify the best-selling models in the dataset.
        
        CAFV Eligibility Distribution: This summarizes the distribution of CAFV eligibility, helping us understand how many vehicles qualify for CAFV incentives.
        
        Electric Vehicle Type Distribution: This shows the breakdown of EV types (e.g., hybrid, fully electric) in the dataset, offering insights into the variety of EVs.
        
        Unique Makes: This operation returns a list of unique EV manufacturers in the dataset.

   Summary Statistics for Categorical Data:

   This provides summary statistics for categorical variables in the dataset, offering insights into the distribution and count of different categories.

   Summary Statistics for Numerical Data:

   This generates summary statistics for numerical variables, such as electric range or price, allowing us to analyze the central tendency, spread, and other metrics.

5. Data Visualization:

   Utilized visual tools like bar charts, histograms, scatter plots, and correlation matrices to interpret data patterns and relationships.

   The following visualizations provide insights into various aspects of the electric vehicle data:

        * EV Model Year Distribution: This count plot illustrates the distribution of electric vehicles by model year.
          It shows the popularity and adoption rates of EV models over time, highlighting years with higher EV production.
        
        * Top 10 Popular EV Models: This horizontal bar chart presents the top 10 most popular electric vehicle models,
          allowing us to identify the models with the highest adoption.
        
        * Cars Per County: This visualization shows the number of electric vehicles registered in different counties,
          which helps understand geographic distribution and county-level adoption of EVs.
        
        * Cars Per City and County: This chart shows the top 15 city and county combinations with the highest number of
          electric vehicles. It provides a detailed look at specific locations where EVs are most prevalent.
        
        * CAFV Eligibility Distribution: This pie chart breaks down the eligibility of electric vehicles for the Clean
          Alternative Fuel Vehicle (CAFV) designation, showing the proportion of eligible and non-eligible vehicles.

   These visualizations provide an in-depth look into the adoption patterns, geographic distribution, and popular models in the electric vehicle dataset.

7. Insights & Results

          EV Adoption Trends: States and cities with higher EV adoption rates were identified.
          
          Range vs. Cost Analysis: Insights into how electric range correlates with MSRP.
          
          CAFV Eligibility Patterns: Analyzed the impact of eligibility for clean alternative fuel designation on EV types.

    Top Findings:

          Most Popular Model Year: The most common model year in the dataset is 2022.
          
          Top 10 EV Makes: The leading EV manufacturers include Tesla, Nissan, Chevrolet, etc.
          
          Top 10 Cities: Cities like Seattle, Bellevue, Redmond, Vancouver, Kirkland, Bothell, Sammamish, Renton, Olympia, Tacoma have the highest adoption rates.
          
          State-Level Insights: California leads the EV adoption trend, with a large percentage of vehicles in the dataset.
          
          Electric Range Trends: Observed the rise in models offering over 300 miles.

          CAFV Incentives: Concentrated in environmentally proactive states like California.

10. Key Findings

          Top EV Model: The Tesla Model 3 is the most popular EV across the dataset.
          
          Geographic Trends: California, New York, and Texas are the top three states with the highest adoption rates.
          
          Electric Range: The average electric range of EVs is increasing, with a significant number of models offering ranges of over 300 miles.
     
4. Libraries Used

        Numpy: For numerical computations.
        
        Pandas: For data manipulation and analysis.
        
        Matplotlib and Seaborn: For data visualization and insight extraction.

# Challenges & Solutions

      Handling Missing Data: Many entries had missing location information. To solve this, imputation techniques and data segmentation were used.
      
      High Dimensionality: The dataset included many categorical variables that required proper encoding. Using label encoding and one-hot encoding helped mitigate this challenge.
      
      Computational Efficiency: Analyzing a large dataset posed computational difficulties. To overcome this, data sampling and efficient pandas operations were employed.

# Limitations

      Data Gaps: Missing values and incomplete data limited some analyses.
      
      Geographic Bias: The dataset may have a bias toward regions with higher EV adoption, affecting the generalizability of the insights.
      
      Temporal Limitations: The data may not reflect recent trends or advancements in EV technology.

# Future Enhancements

      Incorporate More Variables: Adding economic and environmental variables could offer richer insights.
      
      Longitudinal Analysis: Analyze changes in EV trends over time.
      
      Enhanced Geospatial Analysis: Use advanced GIS tools for more detailed geographic insights.

# Conclusion
The Electric Vehicle Data Analysis project provided comprehensive insights into EV adoption, trends, and geographic distribution. The findings highlight the rapid growth of EVs and significant regional differences in adoption rates. Despite some limitations, this analysis offers valuable perspectives for understanding the evolving EV market.

# Contributing
Contributions are welcome! Please open an issue or submit a pull request to contribute.


# Project Milestones

      Highest Electric Range Found: 396 miles (for a Tesla Model S Long Range)
      
      Top 10 EV Models: Tesla Model 3, Nissan Leaf, Chevrolet Bolt, and others.
      
      State with Most EV Adoption: California leads with 30% of total EVs in the dataset.
