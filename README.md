# TLA Data Engineering Task

## Overview

This repository contains a dataset that you, as a candidate for the Data Engineer role at TLA, will use to demonstrate your data handling, cleaning, and transformation skills. The task is designed to simulate real-world scenarios involving dirty data, and you will be required to propose both structured and unstructured solutions.

### Dataset: `TLA_Data_With_Errors.csv`

This CSV file contains vehicle-related data, including:
- **Brand**: Manufacturer of the vehicle (e.g., VOLVO, XEV)
- **Model**: The specific vehicle model (e.g., EX40 ESTATE, YOYO HATCHBACK)
- **Derivative**: Vehicle variant or trim level (e.g., 15kW Pro 10.4kWh 3dr Auto)
- **Introduced**: Date the derivative was introduced
- **Discontinued**: Date the derivative was discontinued (if applicable)

## Task Requirements

You are required to:

1. **Load the Dataset**:  
   Load the `TLA_Data_With_Errors.csv` into a Python environment or any preferred tool.

2. **Data Cleansing**:  
   Identify and resolve errors in the dataset, such as:
   - Missing values
   - Duplicate rows
   - Inconsistent data types
   - Outliers or unrealistic values
   - Misaligned data

3. **Structured and Unstructured Solutions**:  
   Propose and describe how you would store the data in:
   1.	A relational database (e.g., SQL). Suggest a schema and explain how you would set up the tables and relationships. You should also prepare the data in Python, splitting it into the following tables:
	- Brands: Unique brands with BrandID.
	- Models: Unique models with ModelID and a foreign key BrandID.
	- Derivatives: Unique derivatives with DerivativeID and a foreign key ModelID.
	- Vehicle Info: A table containing Introduced, Discontinued, and DerivativeID.

Prepare the data ready to insert into a relational database structure, extract each table as a csv for review?   

   3. An **unstructured or semi-structured format** (e.g., JSON, NoSQL). Provide an example of how the data might be structured in this format.
   4. Technological Recommendations:
	- Explain your choice of technologies for storing, processing, and moving the data (e.g., Azure Event Hub, Databricks, Data Lake Gen 2, or other services).
	- Provide justifications for your recommendations, considering factors like scalability, cost, performance, and maintainability.
	- Where relevant, suggest how these services would work together to form a robust data pipeline.
	- If possible, include a rough cost estimate using the Azure Pricing Calculator or another tool to demonstrate your understanding of resource usage and cost-efficiency.

3. **Bonus (Optional)**:  
   If possible, showcase how you would insert the data into a staging table for further processing and cleansing, and then move it into the final tables.

4. **Documentation**:  
   Include a brief PowerPoint presentation or document that explains:
   - Your approach to cleaning and transforming the data.
   - The steps you took to identify and resolve issues.
   - How you would structure the data for relational and unstructured databases.

## How to Submit

	1.	Reference the dataset:
		• Load the dataset directly using its URL from this repository.
   	'https://raw.githubusercontent.com/YOUR-USERNAME/TLA_Data_Engineering_Task/main/TLA_Data_With_Errors.csv'
	2.	Work through the task:
		• Cleanse and transform the data, as instructed.
		• Provide your scripts, presentation, or documentation explaining your approach and solutions.
	3.	Submit your solution:
		• Upload your solution as a ZIP file, including all your code, documentation, and other relevant files.

Expectations

We are looking for a strong understanding of:

	•	Data cleansing and error resolution.
	•	Best practices for structuring data in relational and non-relational formats.
	•	Clear and concise documentation of your process and solutions.

Additional Information

	•	Feel free to use any tools or libraries you are comfortable with (e.g., pandas in Python, SQL, Excel, etc.).
	•	This task is designed to simulate real-world data engineering challenges, so the focus is on problem-solving and documentation, not perfection.
