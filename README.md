# Capstoneproject
MENTAL HEALTH AT WORKPLACE:
In today's environment, mental wellness is more important than ever. High stress, long hours, work pressure, building a reputation for oneself, and a work-life balance between personal and professional life are all symptoms of mental illness disorder.
We have explored what are the differences in the prevalence of mental disease and attitudes toward mental health by geographic location? What are the most powerful predictors of mental illness in the workplace, as well as specific attitudes regarding mental health? It is important detection and diagnosis of mental health conditions.
This research illuminates the most effective techniques for improving employee wellbeing and encouraging them to seek treatment when necessary.

INITIAL UNDERSTANDING OF THE DATA:

Suppressing warnings to clean up the output.
Importing core libraries and Importing libraries that enable visualization of both the data and the analysis.
Ensuring that matplotlib plots are displayed inline.
Mounting Google Drive to the Colab environment, making files in Google Drive accessible.

UNDERSTANDING THE COLUMNS:

The dataset contains 26 columns in total.The columns are all of object datatype, with the exception of the age column.
Since the comment box was optional, it is logical to assume that the majority of respondents would leave it blank. This is why the comment column appears to have the majority of null values (70%) of all the responses.
Since almost 60% of the population is American, it would be incredibly false to claim that a particular nation has more issues with employee mental health.
Additionally, there are numerous nations with a single response. Thus, the country column loses its meaning. This will be doped. We'll also drop it as a cursory glance at the states indicates that it only applies to those in the US.

DATA PREPARATION & PERFORMING FEATURE ENGINEERING:

In order to see different ages and gender notations in the data, we are printing the different numbers from the 'Age' and 'Gender' columns.
Visualizes missing values in the dataset with a missingno bar plot and adds custom text annotations for context.

EVALUATING MODEL:

In order to maintain the class distribution of the target variable (y) throughout both sets, we are first dividing the dataset into features (X) and target (y). Next, we are using train_test_split to separate the data into training and testing sets, with 30% heading to the test set.
We are creating a dictionary model in which the names of various classification algorithms (such KNeighborsClassifier and LogisticRegression) serve as the keys, and the values are the matching model instances with specific parameters. This makes it simple to retrieve each model by name.
Multiple classification models from the models dictionary are being trained and evaluated. The accuracy of each model on the test set (X_test and y_test) is then calculated, and the accuracy results are appended to the predicted list while the model names and corresponding accuracy scores are printed.

Exploratory Data Analysis (EDA) was conducted using libraries such as matplotlib, seaborn, and plotly for visualization and statistical analysis. Various visualizations, including bar charts, pie charts, and count plots, were created to explore key insights. These included the proportion of employees seeking mental health treatment and the relationships between treatment-seeking behavior and factors like family history, work interference, and remote work. Additionally, missing data was visualized using missingno to ensure that no gaps were overlooked during the analysis.

