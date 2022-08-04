This repository contains the files for my KPMG Data Analytics Consulting Virtual Internship.
The main goal of this project is to work on real data based on a real life business problem. This programme covers all of the key skills of a data analytics consultant: -Data Quality Assessment -Data Insights -Data Insights and Presentation

Summary of The Cleaned Data


Below are more in depth descriptions of data quality issues discovered and methods of
mitigation used. Recommendations and explanations have also been included to avoid further
data quality issues in the future. Following recommendations will improve accuracy of data
used to influence business decisions of Sprocket Central Pty Ltd in the future.


Accuracy Issues 
❖	DOB was inaccurate for "Customer Demographic" and missing an age_column; missing a profit column for "Transactions"

Mitigation: Filter out outlier in DOB.
Recommendation: Create an age_column, allowing for more comprehensible data and easier to check for errors. Create a profit_column in "Transactions" to check accuracy of sales

Creating additional columns for age and profit will allow for easier identification of errors. The profit_column will assist in future monetary analysis.

                                                                                                                                                                         



Completeness
❖	Additional customer ids were inconsistent among *Customer Demographic," **Customer Address," and Transactions"

            Mitigation: Filter all customer_ids from 1 to 3500
            Recommendation: Ensure tables are up to date (from the same time period).


❖	 Blanks in job_title for “Customer Demographic,” in online_order and brand_column for “Transactions”
         Mitigation: Filter out “blanks” for Job_title, Online_order and brand_column.
         Recommendation: simplify Job_title to another category or add dropdowns for all.


Consistency 
❖	Inconsistency in gender for “Customer Demographic” and “Customer Address” respectively. 
         Mitigation: Filter all “M” under “Male” and “Femal” under “Female” for gender.
                               Filter all “New South Wales” to “NSW” and “Victoria” to “VIC” for states.
              Recommendation: provide dropdown options in gender and states.

Currency
❖	People that are “Y” in deceased_indicator are not current customers for “Customer Demographic”
           Mitigation: Filter out customers checked “Y” in deceased_indicator. 

Relevancy
❖	Lack of relevancy or comprehensibility in default_ column for "Customer Demographic" and order status for "Transactions'
         Mitigation: Deleted Metadata in default_column. Filter out 'Cancelled' in         order_status.
         Recommendation: Check for incomprehensible Metadata and delete or format to make comprehensible.



             
Validity
❖	Format of list_price, product _sale_date for *Transactions"
          Mitigation: Format product_sale_date to short date format, format list_price to currency.
          Recommendation: Set up columns so that formats such as price and decimals are already in place when entering new data.


That summaries all data quality issues discovered through the first stage of the data quality
analysis. The mitigation strategies suggested are simple and effective ways of improving data
quality for future analysis. They will not only improve the analysis output that one can
perform within the company but will increase the level of analysis that can be performed by
KPMG and other hired analysis teams.
