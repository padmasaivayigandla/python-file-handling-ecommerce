Python File Handling for E-Commerce Product Management
======================================================

Project Overview:
Efficient management of product information is critical for e-commerce businesses.  
This project demonstrates how Python file handling can be used to read, update, validate, and overwrite data stored in CSV, JSON, and TXT file formats.

The project simulates a real-world e-commerce backend system where:
- Sales data is stored in CSV files
- Product details are stored in JSON files
- Product descriptions are stored in TXT files

Technologies Used:
==================
- Python
- CSV module
- JSON module
- OS module
- Jupyter Notebook

Dataset Description
===================
Sales Data ('sales\_data.csv')
- Contains sales data for multiple products over 14 days
- Each row represents a product
- Columns:
  - Product\_SKU
  - Day1 to Day14
Product Details ('product\_details/')
- Contains JSON files for each product
- Each file is identified by the product SKU
- Stores:
  - Product name
  - Brand
  - Model
  - Specifications
  - Price
  - Availability
Product Descriptions ('product\_descriptions/')
- Contains TXT files
- Each file corresponds to a product SKU
- Stores textual descriptions of products

Functionalities Implemented
===========================
load_data()
- Reads data from:
  - CSV sales file
  - JSON product detail files
  - TXT product description files
- Stores data in dictionaries:
  - 'sales_data'
  - 'product_details'
  - 'product_descriptions'
update_sales_data()
- Adds or updates sales data for a product
- Ensures exactly 14 daily sales values
update_product_details()
- Adds or updates product attributes
- Stores structured product metadata
update_product_description()
- Adds or updates textual product descriptions
update()
- Acts as the main admin function
- Performs validations:
  - SKU must be exactly 13 characters
  - Sales input must contain 14 integers
- Updates all datasets only if validation passes
dump_data()
- Writes updated data back to files
- Automatically creates folders if missing
- Overwrites existing CSV, JSON, and TXT files
- Maintains the original folder structure

How to Run the Project:
1. Clone the repository
2. Navigate to the project folder
3. Open 'file\_handling\_project.ipynb'
4. Run all cells sequentially

Key Learnings:
- Handling multiple file formats using Python
- File system navigation using the 'os' module
- Data validation and error handling
- Modular and reusable function design
- Simulating real-world data pipelines

Author
Padma Sai Vayigandla 
Data Science Learner
