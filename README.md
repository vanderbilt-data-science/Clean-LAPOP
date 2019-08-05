# Clean-LAPOP
This repo contains the data for the Latin American Public Opinion Project. With this information, we aim to create web-based, interactive, self-guided analytics.

## Getting Started
These are the steps you should take to begin using this repo.

### Prerequisites
You will need the current version of [RStudio](https://www.rstudio.com/products/rstudio/#Desktop) to run this code.

Additionally, you will need to download all of the merged files that exist for each country individually from the [LAPOP Datasets](http://datasets.americasbarometer.org/database/index.php)

Finally, you will need the excel file provided by the LAPOP organization that contains the current list of categories and questions to be visualized. The excel file should then be converted to csv for use in RStudio.

These files will need to be placed into the working directory of your project in RStudio.

### Suggested Workflow
1. Reading in Data
    + Reads in the merged country and 2016/17 Stata files downloaded from the [LAPOP Datasets](http://datasets.americasbarometer.org/database/index.php)
    + Creates factored and unfactored versions of all datasets
  
2. Categories and Questions
    + Contains factored and unfactored version of the most recent list of categories and questions provided by LAPOP.

3. Adding Wave Column
    + Creates a column that contains the correct wave for 2016/17 datasets.

4. Creating Unique ID
    + Makes a unique ID for merged country files that follows the unique ID of 2016/17 files.

5. Lengthening and Joining
    + Lengthens countries into tidy format
    + Joins the questions and category columns by column_name

# Team
* Jesse Spencer-Smith | Chief Data Scientist at the Vanderbilt Data Scientist Institute
* Lindsey Fox | Senior IT Consultant for Research
* Carmen Canedo | Vanderbilt Data Science Institute Intern
* Lindsay Hardy | Vanderbilt Data Science Institute Intern
