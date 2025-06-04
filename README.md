# Climate-change

This project, detailed in the focuses on analyzing and modeling data related to climate change, likely from NASA sources.

Key aspects of the project include:

* **Data Loading and Initial Exploration**: The project begins by loading a dataset named "climate_nasa.csv" into a pandas DataFrame. Initial data exploration involves:
    * Displaying the first few rows of the DataFrame.
    * Inspecting data types and non-null counts of columns using `.info()`.
    * Generating descriptive statistics for numerical columns using `.describe()`.
    * The dataset contains columns such as `date`, `likesCount`, `profileName`, `commentsCount`, and `text`.

* **Data Preprocessing**: The notebook addresses missing values by checking for nulls, dropping rows that are entirely null, and filling remaining missing values using a forward-fill method.

* **Exploratory Data Analysis (EDA)**: A visualization step includes plotting the monthly comments count, suggesting an analysis of engagement or discussion trends over time.

* **Machine Learning Model Development**: The project trains a machine learning model, specifically a `RandomForestRegressor`, to potentially predict `commentsCount` based on `likesCount`. This involves:
    * Splitting the data into training and testing sets.
    * Scaling numerical features using `StandardScaler`.
    * Evaluating the model's performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (`r2_score`).
    * Making predictions on new, unseen data.

* **Data Export**: Finally, the cleaned and processed DataFrame is saved to a new CSV file named "Climate_nasa.csv".

The project leverages several Python libraries for its analysis, including `pandas` for data manipulation, `numpy` for numerical operations, `matplotlib.pyplot` and `seaborn` for visualizations, and `scikit-learn` for machine learning tasks.
