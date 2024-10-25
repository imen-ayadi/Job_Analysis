
# Job Offer Salary Analysis Dashboard

This project focuses on analyzing job offers' salary data using Power BI for visualization, combined with Talend for ETL processes. The dashboard provides valuable insights into salary distribution by job title, sector, location, and company size. The project is based on a star schema design, with a fact table for salaries and multiple dimension tables to describe jobs, locations, sectors, and company sizes.

## Dashboard Overview

The dashboard includes the following key visualizations and metrics:

1. **Sum of Average Salaries**: This card displays the total sum of the average salaries across all job offers.
   
2. **Sum of Minimum Salaries**: A card showing the total sum of the minimum salaries for the job offers analyzed.
   
3. **Sum of Maximum Salaries**: The total sum of the maximum salaries offered for the available positions.

4. **Salary by Job Title**: A bar chart showing the top 4 jobs with the highest average salaries, including positions like:
   - Data Scientist
   - Data Engineer
   - Senior Data Scientist
   - Senior Data Engineer

5. **Salary by Sector**: A bar chart visualizing the average, minimum, and maximum salaries across various sectors, including:
   - Information Technology
   - Biotech & Pharmaceuticals
   - Business Services
   - Finance, and more.

6. **Salary by Location**: A bar chart displaying the average salary distribution across different U.S. cities, with notable mentions like:
   - San Francisco, CA
   - New York, NY
   - Cambridge, MA

7. **Number of Job Offers by Company Type**: A breakdown of job offers by the size of the company (large, medium, or small).

## Data Model

This project follows a star schema structure, where the **fact table** contains salary-related information and is linked to multiple **dimension tables** that categorize jobs, locations, sectors, and company sizes.
![Screenshot_49](https://github.com/user-attachments/assets/3fdf6746-9d01-4dc8-aaff-f066a3a6c627)

### Fact Table: `projet_sid_table_fait`

This table stores salary-related metrics:
- `avg_salary`: The average salary offered for the job.
- `min_salary`: The minimum salary offered.
- `max_salary`: The maximum salary offered.
- Foreign keys to the dimension tables (Job, Location, Sector, Size).

### Dimension Tables
- **`projet_sid_dim_job`**: Contains job titles.
- **`projet_sid_dim_location`**: Describes job locations.
- **`projet_sid_dim_sector`**: Holds sector information.
- **`projet_sid_dim_size`**: Contains the company size classification (small, medium, large).

## Technologies Used
- **Talend**: Used for extracting, transforming, and loading (ETL) data into the final format.
- **Power BI**: For data visualization and dashboard creation.
- **SQL**: For database management and data preparation.

## How to Use This Project

1. **Dataset**: The raw data is related to job offers and salary information, classified by job title, location, sector, and company size.
2. **ETL Process**: The data was cleaned and transformed using Talend before loading it into Power BI.
3. **Power BI Dashboard**: The dashboard can be explored to uncover insights into salary distribution by various dimensions.

## Future Enhancements
- Expand the dataset to include more job roles and industries.
- Add time-series analysis to monitor salary trends over time.
- Include filters for more granular data exploration, such as by specific cities or job categories.

## Screenshots

![SID_project](https://github.com/user-attachments/assets/e3dd5673-10d5-4d37-9f7c-40eef05abf3e)

_Description: Job Offer Salary Analysis Dashboard Overview_

---

You can customize the `Dataset` section with more details if you recall the specific transformations done via Talend. Additionally, update the screenshot file path once you upload the relevant images to GitHub. Let me know if you want to include any specific details or sections!
