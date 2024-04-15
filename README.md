# Objective:
- Optimize the weight of the product to be shipped to each warehouse based on historical data.

# Dataset:
- Overview of Dataset: The dataset derives from a fictional noodle company FMCG.It focuses on the instant noodles business and has extensive information related to the instant noodles business. This dataset gives us a valuable information on the demand and supply dynamics with the instant noodle feature.This dataset can be used to create practical solution to reduce inventory expenses and increase the FMCG company total profitability.
## Dataset Variables Description

| Variable                       | Description |
|--------------------------------|-------------|
| `Ware_house_ID`                | Unique identifiers for each warehouse. |
| `WH_Manager_ID`                | Unique identifiers for the warehouse managers. |
| `Location_type`                | Indicates the type of location where each warehouse is situated. |
| `WH_capacity_size`             | Represents the capacity or size of each warehouse. |
| `zone`                         | Categorizes the warehouses into specific zones. |
| `WH_regional_zone`             | Assigns each warehouse to a regional zone. |
| `num_refill_req_l3m`           | Records the number of refill requests received in the last 3 months. |
| `transport_issue_l1y`          | Indicates the occurrence of any transport-related issues within the last year. |
| `Competitor_in_mkt`            | Specifies the presence of competitors in the market. |
| `retail_shop_num`              | Provides the number of retail shops associated with each warehouse. |
| `wh_owner_type`                | Describes the ownership type of each warehouse. |
| `distributor_num`              | Represents the number of distributors associated with each warehouse. |
| `flood_impacted`               | Indicates whether a warehouse has been impacted by floods. |
| `flood_proof`                  | Specifies whether a warehouse is flood-proof. |
| `electric_supply`              | Indicates the status of electric supply to each warehouse. |
| `dist_from_hub`                | Represents the distance of each warehouse from the hub. |
| `workers_num`                  | Provides the number of workers employed at each warehouse. |
| `wh_est_year`                  | Represents the year in which each warehouse was established. |
| `storage_issue_reported_l3m`   | Indicates whether any storage issues have been reported in the last 3 months. |
| `temp_reg_mach`                | Specifies the presence of temperature regulation machinery at each warehouse. |
| `approved_wh_govt_certificate` | Indicates if each warehouse has an approved government certificate. |
| `wh_breakdown_l3m`             | Indicates whether any breakdowns have occurred at each warehouse in the last 3 months. |
| `govt_check_l3m`               | Indicates if government checks have been conducted for each warehouse in the last 3 months. |
| `product_wg_ton`               | Represents the weight of the product in tons. |

## Folder Structure

The project is structured as follows:

```plaintext
FMCG-Supply-Chain-Model/
├── data/                                       # Data directory
│   ├── FMCG_Data.csv                           # Original dataset for FMCG
│   ├── supply_cleaned.csv                      # First cleaned dataset version
│   ├── supply_cleaned2.csv                     # Second cleaned dataset version
│   └── supply_modelingdata.csv                 # Dataset prepared for modeling
│
├── src/                                        # Source code directory
│   ├── task1/                                  # Task 1: Data Cleaning
│   │   ├── task1-data-cleaning.ipynb           # Jupyter notebook for data cleaning
│   │   └── supply_cleaned.csv                  # Output cleaned data from Task 1
│   │
│   ├── task2/                                  # Task 2: Exploratory Data Analysis (EDA)
│   │   └── task2-EDA-Supply-Chain.ipynb        # Jupyter notebook for EDA
│   │
│   ├── task3/                                  # Task 3: Data Preprocessing and Feature Selection
│   │   └── task3-Data-Preprocessing-Feature-Selection.ipynb  # Notebook for preprocessing and feature selection
│   │
│   └── task4/                                  # Task 4: Modeling
│       └── task4-modeling.ipynb                # Jupyter notebook for modeling
│
├── .gitignore                                  # Specifies intentionally untracked files to ignore
├── requirements.txt                            # All necessary dependencies for the project
└── README.md                                   # The README file for the project

