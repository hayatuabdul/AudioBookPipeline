# AudioBookPipeline
A Simple Data Pipeline designed in Python that cleans the data and augments new features to the dataset.

Project Description: Building a Comprehensive Data Cleaning and Feature Augmentation Pipeline using Python

Overview:
In this project, I have conceptualized and implemented an advanced data pipeline using Python, aimed at cleansing and augmenting a dataset containing audio book information. This comprehensive pipeline encompasses multiple functions, each designed to execute distinct data transformation tasks. By skillfully combining these functions, the pipeline ensures the dataset is thoroughly cleansed and enriched, providing an excellent showcase of my data processing capabilities. 

Project Goals: 
The primary objectives of this project were to:

1. Clean and standardize author and narrator names.
2. Convert audio book durations from hours to minutes.
3. Validate and format release dates.
4. Convert price values to floating-point numbers.
5. Extract and process rating-related information.
6. Output the refined dataset to a new CSV file.

Technologies Used:
- Python
- pandas library
- Regular Expressions (re)

Key Features:
1. Author and Narrator Name Cleaning: 
Created functions to remove unwanted prefixes from author and narrator names. Additionally, applied regular expressions to separate first and last names, if required.

2. Duration Conversion:
Converted the duration of audio books from hours and minutes to total minutes. This was accomplished using regular expressions to extract hour and minute components, followed by appropriate calculations.

3. Release Date Validation:
Included a function to convert the 'releasedate' column into a valid datetime format. This ensured uniformity and proper handling of date-related operations.

4. Price Conversion: 
Incorporated a function to convert the 'price' column into floating-point numbers, using a custom 'convert_to_float' method.

5. Rating Extraction and Processing:
Developed functions to extract float values representing ratings from the 'stars' column. Utilized regular expressions to identify and extract relevant numeric information. Calculated the total number of ratings from the same column using a separate function.

6. Output to CSV:
Culminated the pipeline with a function that stored the refined dataset in a new CSV file named 'project_dataset_clean.csv'.

Project Workflow:
1. Loaded the initial dataset ('project_dataset.csv') using the pandas library.
2. Defined functions for cleaning author and narrator names, converting durations, validating release dates, converting prices, extracting ratings, and processing rating-related information.
3. Created a pipeline function ('pipeline()') that executed the cleaning functions sequentially.
4. If executed as the main program, the pipeline function was invoked to perform the comprehensive data cleaning and transformation process.

Skills Demonstrated:
- Proficiency in pandas for data manipulation and transformation.
- Effective use of regular expressions for pattern matching and extraction.
- Handling various data types, including datetime and numeric data.
- Modular code design and organization for complex tasks.
- Utilizing lambda functions for concise transformations.
- Employing the `if __name__ == "__main__":` construct to control script execution.

This project stands as a testament to my adeptness in creating and managing intricate data pipelines. By implementing a range of data cleaning and enrichment tasks, I have demonstrated my ability to handle diverse challenges in data preprocessing, resulting in an enhanced dataset ready for advanced analysis and modeling.
