# Customer-behavioural-Analysis

## Project Summary
An investigation on the behavioral pattern of customers based on their purchasing power, buying habits and their locality can help marketing experts and business stakeholders to make  reliable data-driven decisions surrounding customer’s product preference, target advertisements and service offers in order to meet target demands, beat market competition and inform target marketing. This analytical research focuses on market research based on customer order history for an online retail store which established that total quantity  purchased, and net price are highly correlated than other transactional attributes.

## Aim and Objectives
The end-goal of this research is aimed at leveraging R programming language and studio to 
explore data visualization library tools in order to:
- Validate the correlation between attributes of transactional data.
- Demonstrate sales audit based on product purchased.
- Visually demonstrate consumer purchasing power and buying habits.

## Data Acquisition
The transactional dataset incorporated into this exploratory analysis was retrieved from the repository of University of California, Irvine (UCI), a machine learning database archive that consists of assemblies of database and data generators created by David Aha in 1987 [7]. It consists of a year’s online retail transactions carried out within 01 December 2010 to 09 December 2011 for a UK-registered retail online website. This dataset was gathered from an online dealer that trades assorted gifts with wholesales customers sourced by Dr Daqing Chen, Public analytics Director at the Engineering school at London South Bank University [6]. 

### Data Description 
This dataset comprises of 8 data features with 541909 transactions consisting of real and integer data types which includes customers’ Invoice number; a distinctively allotted 6-digit number for each transaction with a “c” to represent a cancelled transaction, Stock code as the 5-digit product ID string characters allocated to each sales product, a description of each product, the number of quantities sold per transaction, their unit prices, Invoice date as the period when transaction was carried out, uniquely assigned 5-digit customer ID and 36 Country to represent their residential areas which includes Australia, Austria, Bahrain, Belgium, Denmark, Eire, European Community, Brazil, Canada, Channel Islands, RSA, Saudi Arabia, Cyprus, Czech Republic, , Finland, Germany, Greece, Spain, Sweden, Switzerland, United Arab Emirates, United Kingdom, Unspecified, Hong Kong, Iceland, Israel, Italy, Japan, Lebanon, Lithuania, Malta, Netherlands, Norway, Poland, and USA.

![image](https://user-images.githubusercontent.com/76513466/137513807-63247c99-51c6-4fbe-8ae1-e5a4f11d4243.png)

### Data Preprocessing
There are four stages of data preprocessing carried out on the acquired transaction data before data visualization to suit the research purpose as followed below:

• Data reduction: For the time series analysis, online retail transactional data for December 2010 is taken into consideration as point of interest for clear capture and a 
year order history for descriptive analysis for correlation between data features. The Description column was excluded as it does not impact the implementation of data 
visualization and stock codes which are treated as string characters already exist to differentiate each product from another.

![image](https://user-images.githubusercontent.com/76513466/137514054-16587642-4e04-456f-a9dc-35a9678048a9.png)

• Data cleaning: Upon importing the dataset and R libraries, there are 135080 missing cases of Customer ID from the original dataset of 541909 transactions and the complete.case() command function was invoked to remove these missing ID as they are character numbers unique to different customers and cannot be precisely predicted to avoid noisy data.

![image](https://user-images.githubusercontent.com/76513466/137514177-ad4ee83a-582c-4774-abb3-ea04163bb34c.png)

• Data transformation: The aggregate of the month of December was taken for the exploratory analysis by creating a pivot table and grouping the data attributes into rows and column values to cumulate the transactions within each day and for each unique customer ID. The time format was also changed from a date-time structure, day/month/year to a day/month layout with the Lubridate library from R studio.

![image](https://user-images.githubusercontent.com/76513466/137514347-2745c09c-fa7f-4027-99d5-e5e94761f511.png)

## Data Visualization
In order to achieve the aim of this research, data visualization tools that includes Density plot, 3D Scatterplot and correlation matrix plot to detect association and patterns between features of online consumer’s transactional data and spot outliers with a point chart for clear and concise display of dataset.

### Density Plot
The aggregate of a month’s transaction data was obtained before plotting the density chart to display total quantities of product purchased daily in December 2010.

![image](https://user-images.githubusercontent.com/76513466/137514832-34e378f0-dda1-4eaf-8127-6b1db89e92b4.png)

### 3D Scatterplot
 A three-dimensional chart displaying the relationship between Customer ID, Net price and invoice number to observe for example, whether the arrangement of invoice number affects product sales and so on.

                          Figure 7: 3D plot of Customer’s Net purchases
![image](https://user-images.githubusercontent.com/76513466/137515170-9341e683-0698-468a-82b8-bb05c28ab874.png)

### Correlation Matrix
 It also denotes the transaction data attributes with the highest correlation coefficients whether positive (1) or negative (-1) to examine whether these features are dependent of one another or independent.

![image](https://user-images.githubusercontent.com/76513466/137515360-b9f634b6-4417-47da-82ba-61885a84eac9.png)

## Conclusion
An enquiry into customer’s behavioral pattern by integrating transaction history with data visualization tools will not only provide insights on trends and patterns on customer’s purchasing power and buying habits but also inform market advertising, business decisions in this case online retail store and attract more online customers to drive business growth. This analysis will also aid retailers to improve in the area of customer relationship management and monitor customer satisfaction and business performance. Further research on this project can be done on investigating the sales period and customer’s activities on the aspect of time series analysis with the formatted dates to forecast future sales and product demand as well as product classification and clustering with data mining techniques.








