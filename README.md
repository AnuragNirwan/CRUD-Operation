## Introduction <br>
Efficient and accurate management of product information is vital for the success of e-commerce businesses. Reliable product data not only facilitates informed decision-making but also drives effective marketing strategies. Traditional methods of managing product data, such as manual entry and maintenance, are often cumbersome and error-prone. These inefficiencies can lead to data inconsistencies, operational delays, and lost business opportunities. <br>

To address these challenges, leveraging Python programming offers a robust solution. Python's capabilities allow for the development of automated systems that handle core operations such as adding, retrieving, updating, and deleting product information. By automating these CRUD (Create, Retrieve, Update, and Delete) operations, businesses can improve data accuracy, streamline workflows, and boost overall efficiency. <br>

CRUD Operations Overview <br>
CRUD represents the fundamental operations required to manage data in any application, whether it's for a database, data storage system, or software. Each operation plays a distinct role in data management:<br>

**Create:** Adds new records to a database or data structure. Example: Adding a new product or user profile to a database. <br>
**Read:** Fetches or queries data from a database based on specific criteria. Example: Retrieving all product details or sales data. <br>
**Update:** Modifies existing records to reflect changes. Example: Updating the price of a product or correcting a user’s contact details. <br>
**Delete:** Removes records from the system to maintain a clean and relevant database. Example: Deleting outdated or redundant product information. <br>


These operations form the backbone of data-driven systems, ensuring data is accessible, accurate, and up-to-date.

**Project Implementation:** Customizing CRUD Operations
In this project, Python is used to implement a customized version of CRUD operations tailored to e-commerce data management. The implementation includes managing sales data, product details, and product descriptions.

### 1. Create Operation <br>
The create() function orchestrates data entry tasks through the following sub-functions: <br>

**add_sales_data():** Records sales data such as transactions or revenue. <br>
**add_product_details():** Stores essential product information (e.g., name, SKU, price). <br>
**add_product_descriptions():** Captures descriptive details like features or specifications. <br>

### 2. Read Operation <br>
The read() function retrieves and displays data using these sub-functions: <br>

**display_sales_data():** Presents sales-related insights or records. <br>
**display_product_details():** Outputs key product details for analysis or review. <br>
**display_product_descriptions():** Displays detailed product descriptions for marketing or customer reference. <br>


### 3. Update Operation <br>
The update() function allows modifications to existing data via: <br>

**update_sales_data():** Updates sales records, such as adjustments to revenue or transactions.<br>
**update_product_details():** Modifies product attributes like pricing or availability. <br>
**update_product_descriptions():** Refines or adds details to product descriptions. <br>


### 4. Delete Operation <br>
**The delete():** function manages data removal processes to keep the system organized and relevant. It ensures that obsolete or unnecessary records are efficiently removed. <br>

## 5. Central CRUD Function <br>
The crud() function serves as the project's core, seamlessly coordinating all CRUD operations. This master function provides a unified interface for executing Create, Read, Update, and Delete tasks, making it user-friendly and highly efficient.

### Benefits of This Approach <br>

**1. Improved Accuracy:**  Automation reduces manual errors, ensuring reliable data.<br>
**2. Enhanced Efficiency:** Streamlined workflows save time and resources.<br>
**3. Scalability:** The system can handle increasing data volumes as the business grows. <br>
**4. Centralized Management:** The crud() function simplifies interaction with the data system. <br>

By implementing this Python-based CRUD system, e-commerce businesses can unlock new levels of operational excellence, ensuring their product information is well-managed, accurate, and readily accessible. This approach not only optimizes current operations but also positions the business for future scalability and success.

## Problem Statement <br>
In the dynamic landscape of e-commerce, efficient management of product information is essential for businesses to thrive. However, organizing and updating vast arrays of product details, sales data, and product descriptions can be a daunting task without the right tools in place. The absence of a robust system for managing product information can lead to inconsistencies, errors, and inefficiencies in operations.<br>

To address this problem, you have been hired as a software developer for a Software company that builds various technologies for e-commerce platforms. Your job is to utilize your programming knowledge to automate some of the tasks that occur in these e-commerce platforms. Specifically, your role involves implementing functionalities for seamlessly adding, reading, updating, and deleting product details, sales data, and product descriptions. <br>

## Understanding the Data <br>

**1.** You have one main folder called main_folder containing one CSV file and 2 subfolders called product_details and product_description. The sales_data.csv contains sales data for various products over 14 days. Each row represents a unique product identified by its Product_SKU, and each column represents the number of sales for that product on a specific day (Day1 to Day14). The values in the cells indicate the number of units sold for each product on the corresponding day. <br>

**2.** The product_details folder contains JSON files named after each product's SKU (e.g., details_AISJDKFJW93NJ.json, details_DJKFIEI432FIE.json). These JSON files contain detailed information about each product, such as its name, brand, model, specifications, price, and availability. For example, take a look at the below screenshot of the JSON file details_AISJDKFJW93NJ.json. <br>

**3.** The product_description folder contains TXT files named after each product's SKU (e.g., description_AISJDKFJW93NJ.txt, description_DJKFIEI432FIE.txt). These TXT files contain descriptions of each product. For example, take a look at the below screenshot of the TXT file description_AISJDKFJW93NJ.txt. <br>


### TASK
**Q1: Your first task is to set up the environment for this project by loading the required packages and modules.** <br>
You will achieve all of this by completing the following sub-task: <br>

1. Write code to import the following packages: <br>
- For handling raw data files: os <br>
- For working with JSON files: json <br>
- For working with CSV files: csv <br>
- For pretty-printing Python data structures: pprint <br>

**Q2: Then, you will ensure that the necessary files are loaded into the working environment. This includes loading sales data from a CSV file, product details from JSON files, and product descriptions from text files.** <br> 

We recommend that you either use Jupyter Notebook or Google Colab to build and execute your code. You will achieve all of this by completing the following tasks: <br>
1. In case you are using Google Colab, <br>
- import drive from google.colab and mount your Google Drive or <br>
- import files from google.colab. <br>
2. In case you are using Jupyter Notebook, please make sure that your files and folders are all in the right place. <br>
3. Use a function named load_data() to read data from the sales_data.csv file, JSON files in the product_details folder, and TXT files in the product_description folder and store them in three dictionaries called sales_data, product_details and product_desctiptions. <br>

**Q3: Next, you will explore the loaded data by displaying its content. This includes displaying sales data, product details, and product description of products using their product SKU.** <br>

You will perform the following in this task: <br>

1. Display sales_data, product_details, and product_descriptions dictionaries. <br>
2. Create a list named product_skus which contains product SKUs extracted from one of the dictionaries using dict.keys(). <br>
3. Display sales data, product details, and product description of a product using the product_skus list. <br>
4.Find the length of sales_data, product_details, and product_descriptions dictionaries. <br>

**Q4: A new laptop model, the Acer Aspire 3, laptop has been launched by Acer.  Your task is to create a function that lets the admin add sales data, product details, and product description for this new product.** <br>

The code should help the admin to accomplish the following tasks:<br>

1. Use a function named add_sales_data() to add sales data for Acer Aspire 3, which has the following sales data:<br>
- Product SKU: TYS56KFJW93NJ
- Sales data for the past 14 days:  [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]

2. Use a function named add_product_details() to add new product details for Acer Aspire 3, which has the following product details: <br>
- Product name: Laptop <br>
- Brand: Acer <br>
- Model: Acer Aspire 3 <br>
- Specifications: Intel Core i3 N305 Laptop (Windows 11 Home/8 GB/512 GB SSD) A314-36M, 35.56 cm (14") Full HD Display, 1.4 KG, Pure Silver <br>
- Price: INR 32,999.00 <br>
- Availability: In stock <br>

3. Use a function named add_product_description() to add a product description for Acer Aspire 3, which has the following product description: <br>
- Product Description: The Aspire 3 is ready to go with the latest Intel® Core™ i3 N-Series Processors1 with UHD Graphics—ideal for the entire family, with performance and productivity at the core. Perfect to get more out of work, study, or play. <br>

4. Use a function named create() that calls the functions defined in 1, 2, and 3 to add product details, sales data, and product descriptions for the Acer Aspire 3 laptop at once.

**Q5: Let’s say the admin wants to review the details of the Acer Aspire 3 laptop before making any updates. In this case, you'll create functions to allow the admin to display the sales data, product details, and product description of the Acer Aspire 3 laptop.** <br>

The code should help the admin to accomplish the following tasks:<br>
1. Use a function named display_sales_data() to display sales data for Acer Aspire 3.<br>
2. Use a function named display_product_details() to display product details for Acer Aspire 3. <br>
3. Use a function named display_product_descriptions() to display product description for Acer Aspire 3. <br>
4. Use a function named read() that calls the functions defined in 1, 2, and 3 to display sales data, product details, and product descriptions for Acer Aspire 3 at once. <br>

**Q6: Acer decides to release a software update for the Acer Aspire 3 laptop, which includes performance enhancements, new features and price increases. In this task, you will implement functionality to let the admin update sales data, product details, and product description.** <br> 

The code should help the admin to accomplish the following tasks:<br>
1. Use a function named update_sales_data() to update sales data for Acer Aspire 3 <br>
2. Use a function named update_product_details() to update product details for Acer Aspire 3. <br>
3. Use a function named update_product_descriptions() to update the product description for Acer Aspire 3. <br>
4. Use a function named update() that calls the functions defined in 1, 2, and 3 to update sales data, product details, and product descriptions for Acer Aspire 3 at once. <br>

**Q7: Suppose Acer discontinues the production of the Acer Aspire 3 laptop due to the release of its successor, the Acer Aspire 4.  The admin wants to remove all information related to the Acer Aspire 3. In this task, you will implement functionality to let the admin delete sales data, product details, and product description.** <br>

The code should help the admin to accomplish the following task:<br>
1. Use a function named delete() to delete sales data, product details, and product descriptions for Acer Aspire 3 whose product SKU is TYS56KFJW93NJ at once.
