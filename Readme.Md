# Objective : Create the python script to generate fake transactional data.
- Create amount for each cart and quantity of products
- Aggregate the features
- Export the new dataset as a CSV

# Requirements : Generate transactionnal data
1. A transaction may contain multiple products
2. The fake data should contain some loyal shoppers
3. A product quantity of 0 indicates it references a service.
4. A transaction status may have one of the following values : Confirmed, Concelled, Pending

# Important : Before using the script "data_generation.py"

 - The .env file must be at the root directory of this project
 - All the variables in the .env file are mandatory 
 - Set the values of all the required variables 
 - The 'Config' class is in charge of reading and loading the enviremental variables
 - The generated data file could be found under the 'output' directory
 - The log file is called 'app.log' and could be found under the 'logs' directory

# Transaction data example 

Below is an example of data describing a shopping transaction. A shopper may purchase multiple products. Each transaction includes a date and status, along with product details stored as a list of 'products'.

{ "shopper_id": "12345", "transaction_date": "2024-03-01", "order_status": "Confirmed",
"final_ati_amount": "100.00", "products": [{"product_id": "A100", "unit_ati_amount":
"50.00", "quantity": 2}] }

