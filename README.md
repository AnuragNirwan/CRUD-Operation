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
