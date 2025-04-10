👋 Hi there! I’m a Computer Science and Economics student at Northeastern University, passionate about leveraging data science, machine learning, and software engineering to build impactful solutions. My interests include data engineering, predictive modeling, and software development, where I explore creative approaches to solving problems.

Projects & Highlights:
- NHL Salary Prediction Model: Developed a predictive model using Python, SQL, and XGBoost to analyze over 800 player datasets. Focused on data cleaning, feature engineering, and visualization to deliver actionable insights about salary forecasting.
- Interactive Spelling Bee Game: Designed and implemented a web-based spelling bee game using Python and Flask. The project combines natural language processing and gamification principles to create an engaging and educational user experience.

I love tackling complex challenges with scalable, data-driven solutions and enjoy collaborating on projects that combine technical expertise with creativity. Feel free to connect or explore my repositories for more details on my work!



Check out some of my other work in my 'AdditionalProjects' repository: https://github.com/DanMccue/AdditionalProjects


# NHL Player Salary Analysis Project

<img width="550" alt="image" src="https://github.com/user-attachments/assets/0242df09-ef41-464b-817d-15209c16d302" /> <img width="450" alt="image" src="https://github.com/user-attachments/assets/6bba4925-861d-428c-90cc-697bc8af18fc" />




Overview:

- A machine learning analysis of NHL player salaries using performance metrics to predict compensation and identify market inefficiencies, using XGBoost and Lasso regression models.



Dataset:

- 789 NHL players from 2016-17 season

- 154 performance features including:

	- Traditional stats (Goals, Assists, Points)

	- Advanced metrics (Fenwick, Corsi)

	- Physical attributes (Height, Weight)

 	- Career statistics (Experience, Draft position)

  	- Salary range: $575K to $14M

 

Methodology:

Data Preprocessing

- Age calculation from birth dates

- Experience derivation from draft years

- Position standardization (Defense/Center/Wing)

- Draft position normalization

- Advanced metric computation

- Handling of undrafted players



Model Development

- Implemented XGBoost and Lasso regression models

- Cross-validation with 5 folds

- Hyperparameter optimization

- Feature importance analysis



Results:

Model Performance

- Lasso Regression achieved 47.0% accuracy (R² = 0.470 ± 0.030) with RMSE of $1.69M

- XGBoost achieved 44.5% accuracy (R² = 0.445 ± 0.058) with RMSE of $1.73M

Key Predictors

- Flow Statistics

	- Fenwick For (FF): Strongest predictor
	
 	- Corsi For (CF): Third most important

	- Individual Shots (iSF)

- Scoring Metrics

	- Goals Scored (GS): Second strongest predictor

	- Expected Goals For (xGF)

	- Points (PTS)
 
Salary Analysis

- Most efficient team: Carolina Hurricanes underpaying by $0.84M per player average

- Least efficient team: Buffalo Sabres overpaying by $0.55M average

Notable Contract Discrepancies (predicted salary in millions)

- Highest Overpaid: Stamkos ($7.83M), Kopitar ($7.52M), Toews ($7.21M)

- Most Underpaid: Panarin ($4.37M), Slavin ($4.34M), Gostisbehere ($4.27M)

Market Inefficiencies

- Entry Level Contracts significantly undervalue young talent

- Veteran contracts often exceed statistical performance value

- Teams with efficient salary structures tend to maximize performance metrics relative to payroll



Limitations:

- Single season analysis

- Actual salary vs cap hit consideration

- Unquantifiable factors (leadership, marketability, reputation)
  
- Entry-level contract restrictions


Author:
Daniel Mccue
 - Last Updated: January 2025
