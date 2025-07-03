Titanic-EDA-Jupyter

📄 Overview
This repository contains an Exploratory Data Analysis (EDA) of the famous Titanic disaster dataset. The project aims to uncover patterns and relationships within the data to understand the factors that influenced survival rates. Conducted entirely within a Jupyter Notebook, this analysis showcases data cleaning, preprocessing, univariate and bivariate analysis, advanced visualizations, and basic interactive elements using ipywidgets.

🎯 Project Goals
The main objectives of this EDA project are:

Data Understanding: Load and inspect the dataset to understand its structure, data types, and identify missing values.

Data Cleaning & Preprocessing: Handle missing data and engineer new features that could be insightful for analysis.

Feature Analysis: Explore individual features (e.g., Age, Sex, Pclass, Fare) and their distributions.

Survival Factor Identification: Investigate how different features correlate with the Survived target variable.

Data Visualization: Create compelling visualizations using Matplotlib and Seaborn to communicate findings effectively.

Interactive Exploration: Implement basic ipywidgets to allow dynamic filtering and exploration of the data.

Storytelling: Summarize key insights and present a clear narrative of the findings.

📊 Dataset
The dataset used in this project is the train.csv file from the Kaggle "Titanic - Machine Learning from Disaster" competition. It contains various details about the passengers on the Titanic, including:

PassengerId: A unique identifier for each passenger.

Survived: Survival status (0 = No, 1 = Yes). This is the target variable.

Pclass: Passenger Class (1 = 1st, 2 = 2nd, 3 = 3rd).

Name: Passenger's name.

Sex: Passenger's gender.

Age: Passenger's age in years.

SibSp: Number of siblings/spouses aboard the Titanic.

Parch: Number of parents/children aboard the Titanic.

Ticket: Ticket number.

Fare: Passenger fare.

Cabin: Cabin number.

Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

Source: Kaggle Titanic Dataset

🛠️ Tools & Technologies
This project is developed using:

Jupyter Notebook / JupyterLab: The interactive environment for writing and executing code.

Python 3: The primary programming language.

Pandas: For data manipulation and analysis.

NumPy: For numerical operations.

Matplotlib: For basic plotting and plot customization.

Seaborn: For creating high-level statistical visualizations.

ipywidgets: For adding interactive controls to the notebook.

📈 Analysis Performed
The Titanic_EDA_Jupyter.ipynb notebook covers the following analytical steps:

Initial Data Loading and Inspection: Using df.head(), df.info(), and df.describe() to get a first look at the data.

Missing Value Handling: Imputing Age with the median, Embarked with the mode, and dropping the Cabin column due to excessive missingness.

Feature Engineering:

Creating FamilySize from SibSp and Parch.

Deriving IsAlone from FamilySize.

Extracting and consolidating Title from the Name column.

Univariate Analysis: Visualizing the distribution of individual features like Age, Fare, Sex, Pclass, and the Survived target variable.

Bivariate Analysis: Exploring the relationship between Survived and other features (e.g., Sex vs. Survived, Pclass vs. Survived, Age vs. Survived, Fare vs. Survived, FamilySize vs. Survived, Title vs. Survived).

Advanced Visualizations: Utilizing seaborn.pairplot for a comprehensive look at relationships between numerical features.

Interactive Filters: Implementing ipywidgets to create interactive sliders for filtering age and fare ranges, allowing dynamic updates to distribution plots.

🔑 Key Insights
The exploratory data analysis revealed several significant factors influencing survival on the Titanic:

Gender was the most dominant factor: Females had a substantially higher survival rate than males, consistent with the "women and children first" protocol.

Socio-economic status played a critical role: Passengers in higher classes (1st and 2nd) had significantly better survival chances compared to 3rd class passengers, often correlated with higher fares and better access to lifeboats.

Age had a nuanced impact: Very young children (e.g., under 10) showed a higher propensity for survival.

Family dynamics mattered: Passengers traveling alone or in very large groups had lower survival rates compared to those in small to medium-sized families.

Social titles reflected survival chances: Titles indicating higher social standing or marital status (e.g., 'Mrs.', 'Master') generally correlated with better survival rates.

🚀 How to Run the Notebook
To run this project on your local machine, follow these steps:

1. Clone the Repository
git clone https://github.com/YourGitHubUsername/Titanic-EDA-Jupyter.git
cd Titanic-EDA-Jupyter

(Remember to replace YourGitHubUsername with your actual GitHub username)

2. Download the Dataset
Go to the Kaggle Titanic Dataset page.

Download the train.csv file.

Place train.csv directly into the Titanic-EDA-Jupyter directory you just cloned.

3. Set Up Your Environment
It is highly recommended to use Anaconda for managing your Python environment.

Install Anaconda: If you don't have it, download and install Anaconda from anaconda.com/download.

Create and Activate a Conda Environment (Recommended):

conda create -n titanic_env python=3.9
conda activate titanic_env

Install Required Libraries:

conda install pandas numpy matplotlib seaborn jupyter ipywidgets -c conda-forge

(The -c conda-forge is important for ipywidgets compatibility.)

Enable ipywidgets extensions (Crucial for interactivity):

For Jupyter Notebook:

jupyter nbextension enable --py widgetsnbextension --sys-prefix

For JupyterLab:

jupyter labextension install @jupyter-widgets/jupyterlab-manager

You might need to restart your terminal/Anaconda Prompt after these commands.

4. Launch Jupyter Notebook / JupyterLab
From the Titanic-EDA-Jupyter directory in your terminal/Anaconda Prompt:

jupyter notebook
# OR
# jupyter lab

This will open Jupyter in your web browser.

5. Open and Run the Notebook
In the Jupyter interface, navigate to and open Titanic_EDA_Jupyter.ipynb.

You can run the cells one by one by selecting a cell and pressing Shift + Enter, or run all cells via Cell > Run All.

🤝 Contributing
Feel free to fork this repository, make improvements, and submit pull requests. Any suggestions for further analysis or visualization are welcome!

📄 License
This project is open-source and available under the MIT License.