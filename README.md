# PLSQL-Cultural_and_Heritage_Management_System-Zensar
# Cultural Heritage Management System
## About Me
Hello! I am Shrushti Khemnar, a third-year *Computer Engineering* student at *AVCOE College*.

## Description
This project is a database system designed to manage cultural heritage sites, artifacts, restoration projects, and visitor records. The system ensures efficient operations and the preservation of cultural heritage while providing analytics for better decision-making.

## Features

### 1. Heritage Data Management
- Tables for managing data related to cultural heritage sites, artifacts, and restoration projects.
- Triggers to log updates and maintain historical data for transparency and record-keeping.

### 2. Visitor Analytics
- Procedures to track visitor numbers and calculate revenue.
- Generate reports on the most popular heritage sites to assist in decision-making and marketing.

### 3. Restoration Monitoring
- Functions to calculate restoration project costs.
- Triggers to alert administrators about project delays or funding shortages.

## Database Schema

The database includes the following key tables:
- `Sites`: Stores information about cultural heritage sites.
- `Artifacts`: Contains details of artifacts related to the sites.
- `Restoration`: Tracks restoration projects, including their progress and costs.
- `Visitors`: Logs visitor data, including numbers and revenue generated.

## Getting Started

### Prerequisites
- A relational database management system (e.g., MySQL, PostgreSQL, Oracle, etc.).
- Basic knowledge of SQL and PL/SQL (if applicable).

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heritage-db-system.git
   cd heritage-db-system
   ```
2. Import the database schema:
   ```sql
   SOURCE schema.sql;
   ```
3. Load sample data (optional):
   ```sql
   SOURCE sample_data.sql;
   ```

## Usage

### Heritage Data Management
- Add or update data about sites, artifacts, or restoration projects using the provided SQL scripts.
- Historical changes are logged automatically using triggers.

### Visitor Analytics
- Run the `calculate_revenue` procedure to compute total revenue.
- Use the `popular_sites_report` procedure to generate reports on popular sites.

### Restoration Monitoring
- Use the `calculate_project_cost` function to estimate restoration project expenses.
- Delays or funding shortages trigger alerts for immediate action.

## Example Queries

### Adding a New Site
```sql
INSERT INTO Sites (site_id, name, location, description) 
VALUES (1, 'Ancient Ruins', 'City A', 'Historical ruins dating back to 500 BC');
```

### Calculating Total Revenue
```sql
CALL calculate_revenue();
```

### Generating Popular Sites Report
```sql
CALL popular_sites_report();
```

### Checking Restoration Costs
```sql
SELECT calculate_project_cost(1); -- Where 1 is the project ID
```

## Triggers and Alerts
- **Update Logging:** Logs every update to heritage site or artifact data.
- **Restoration Alerts:** Notifies about delays or funding issues in restoration projects.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with detailed changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more information.

## Acknowledgments
- Inspiration for this project came from the need to preserve and efficiently manage cultural heritage.
- Thanks to all contributors and supporters of the project.

