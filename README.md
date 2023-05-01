# FIFA '21 Data Cleaning Challenge
<div align="center">
  <img src="https://github.com/toheebolamilekn/fifa21_data_cleaning_challenge/blob/main/fifa21_logo.jpg" width="1000" height="400"/>
</div>

---
### Introduction
- According to [Wikipedia](https://en.wikipedia.org/wiki/Data_cleansing), Data cleaning or cleansing is the process of detecting and correcting (or removing) corrupt or inaccurate records from a record set, table, or database and refers to identifying incomplete, incorrect, inaccurate or irrelevant parts of the data and then replacing, modifying, or deleting the dirty or coarse data. Data cleansing may be performed interactively with data wrangling tools such as Python, R, SQL, Microsoft Excel, Power Query in Excel or in Power BI or as batch processing through scripting or a data quality firewall.

- After cleansing, a data set should be consistent with other similar data sets in the system. The inconsistencies detected or removed may have been originally caused by user entry errors, by corruption in transmission or storage, or by different data dictionary definitions of similar entities in different stores. Data cleaning differs from data validation in that validation almost invariably means data is rejected from the system at entry and is performed at the time of entry, rather than on batches of data.

- The actual process of data cleansing may involve removing typographical errors or validating and correcting values against a known list of entities. The validation may be strict (such as rejecting any address that does not have a valid postal code), or with fuzzy or approximate string matching (such as correcting records that partially match existing, known records). Some data cleansing solutions will clean data by cross-checking with a validated data set. A common data cleansing practice is data enhancement, where data is made more complete by adding related information. For example, appending addresses with any phone numbers related to that address. Data cleansing may also involve harmonization (or normalization) of data, which is the process of bringing together data of "varying file formats, naming conventions, and columns", and transforming it into one cohesive data set; a simple example is the expansion of abbreviations ("st, rd, etc." to "street, road, etcetera").
---
### About the dataset
- The raw dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring/code) via web scrapping from sofifa.com which can also be access here [fifa21_raw_data_v2](https://github.com/toheebolamilekn/fifa21_data_cleaning_challenge/blob/main/fifa21_raw_data_v2.csv). It consists of all information concerning football players such as player names, age, clubs, nationality, wages, positions, performance ratings, height & weight etc. The raw dataset before cleaning consists of 18979 rows and 76 columns. The cleaned dataset set consists of 18979 rows and 72 columns.
#### Note: python rows and columns counting start from zero (0) not one (1).
---
### Objectives
- The main objective of this data challenge was to learn, improve skills and network with like-mind and get to build a worthy-portfolio project. 
- Other specific objectives are stated below;
 1. Ensure that all the columns have the correct data type.
 2. Numerical columns should be in a format suitable for further calculations and analysis.
- In order to achieve the aforementioned objectives, we are to;
 1. Ensure correct data types, 
 2. Correct inconsistent naming of column and/or values,
 3. Check for null entries and missing entries, 
 4. Remove unnecessary characters as well as irrelevant column.
---
### Process
- The step by step process were perfectly explained together with the cleaning process in Python Jupiter Notebook which can be found uploaded above named [FIFA '21 Messy Raw Dataset Cleaning Challenge](https://github.com/toheebolamilekn/fifa21_data_cleaning_challenge/blob/main/FIFA%20'21%20Messy%20Raw%20Dataset%20Cleaning%20Challenge.ipynb).
---
### Conclusion
The data cleaning analysis explained in the previous section and presented in Python Jupiter Notebook file allow us to draw some conclusion about each of the objectives raised at the beginning of this data cleaning challenge.
- First, on the main objective of this data cleaning challenge to learn, improve skills, network with like-mind and get to build a worthy-portfolio project. We can conclude on the basis of evidence provided by the csv file exported from Python Jupiter Notebook at the end of the data cleaning which was uploaded in the repository [fifa21_cleaned_data](https://github.com/toheebolamilekn/fifa21_data_cleaning_challenge/blob/main/fifa21_cleaned_data.csv). Several data community were created by the two hosts [Promise Chinonso](https://twitter.com/PromiseNonso_) and [Victor Somadina](https://twitter.com/vicSomadina) of the data cleaning challenge which include Twitter using the hashtag (#datacleaningchallenge) and also Telegram sub-groups for several data cleaning tools depends on which tool ones preferred to use for the data cleaning challenge such as Microsoft Excel, Power Query, Python, R, SQL etc. to connect with peers, learn from and guide each other, share day-by-day progress, sharpen/improve one’s skills to build worthy- portfolio project as well as share finished data cleaning project or portfolio URL.
- Second, on the specific objective to ensure that all the columns have the correct data type. The fifa_df.info() revealed that the dataset only had two data types (53 int64 {whole number} and 23 object {string or non-numeric}) before the data cleaning process. The data type were corrected along the data cleaning process and at the end of the data cleaning, fifa_df.info() now revealed that the cleaned dataset consists of five data types which are `(category(1), datetime64[ns](1), int64(59) and object(11))`.
- Lastly, on the second specific objective to ensure numerical columns be in a format suitable for further calculations and analysis. This was achieve by defining several function during the data cleaning process to convert some inconsistent column values to specific/consistent values such as all_to_cm, all_to_kg, pd.to_datetime() and also for loop to remove unnecessary special characters from the column values using `fifa_df[‘ ’].str.split(), fifa_df[‘ ’].str.slice(), fifa_df[‘ ’].str.slip(), fifa_df[‘ ’].str.rslip(), fifa_df[‘ ’].str.lslip(), fifa_df.replace(), fifa_df.drop()` etc.
---
- Now, we are ready to use the cleaned dataset for further analysis and visualization.
- For further suggestion or inquiries, please feel free to contact me on [LinkedIn](https://www.linkedin.com/in/toheebolamilekan) and [Twitter](https://twitter.com/toheebolamilekn).
