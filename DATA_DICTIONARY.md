# Data Dictionary

This document provides details on the fields found in the source CSV files.

### `Power_Plant_Data_2019-21.csv` & `Power_Plant_Data_2022-25.csv`

| Column Name             | Description                                                                 | Data Type |
| ----------------------- | --------------------------------------------------------------------------- | --------- |
| `Order ID`              | A unique identifier for each order. Primary key.                            | String    |
| `Product ID`            | A unique identifier for each product.                                       | String    |
| `Order Date`            | The date the order was placed.                                              | Date      |
| `Production date`       | The date the product manufacturing was completed.                           | Date      |
| `Actual Delivery Date`  | The date the order was actually delivered to the customer. (Blank if not yet delivered) | Date      |
| `Estimated Delivery Date` | The planned date of delivery.                                               | Date      |
| `Chemical Grade`        | The grade of the chemical ordered (e.g., E-Grade, Toxic, Low, Standard).    | String    |
| `Production Location`   | The plant facility where the product was made (e.g., Foundary, Packaging).  | String    |
| `Delivery State`        | The state to which the order was delivered.                                 | String    |
| `Delivery City`         | The city to which the order was delivered.                                  | String    |
| `Country`               | The country to which the order was delivered.                               | String    |

### `Power_Plant_Order_Status.csv`

| Column Name       | Description                                                 | Data Type |
| ----------------- | ----------------------------------------------------------- | --------- |
| `Order ID`        | A unique identifier for each order. Foreign key.            | String    |
| `Order Status - 1`| The detailed status of the order (e.g., Completed - Late).  | String    |
| `Order Status - 2`| The summary status of the order (Complete or Incomplete).   | String    |
