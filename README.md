## Freight Management System

This **Python** project implements a basic freight management system using **SQLite** to track container capacity and cargo details, enabling users to simulate loading scenarios and analyze key performance indicators (KPIs).

### Features

* **Box Type Management:** Define and store dimensions (height, width, length) of various box types.
* **Container Loading Simulation:** Assign boxes to containers, with built-in capacity checks to prevent overloading.
* **Freight Tracking:** Maintain a record of which boxes are assigned to which containers.
* **Summary Reporting:** Generate reports that include:
    * Total number of containers used.
    * Total contracted volume.
    * Estimated transportation cost based on container usage and volume.
    * Projected profit/loss. 

### Project Motivation

This project was developed to demonstrate practical applications of data engineering concepts, including:

* **Data Modeling:** Design a relational database schema to efficiently store and manage freight-related data.
* **SQL Interaction:** Implement CRUD (Create, Read, Update, Delete) operations and data retrieval using SQL queries.
* **Python for Data Management:** Use Python to interact with the database, implement business logic, and present data. 

### Technical Implementation

* **Language:** Python 3.6+
* **Database:** SQLite3
* **Libraries:** `sqlite3` (built-in), `tabulate` (for formatted output)

### How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/freight-management-system.git 
   cd freight-management-system
   ```
2. **Run the application:** 
   ```bash
   python interface.py 
   ```
3. **Interact with the system:**  Follow the menu-driven command-line interface to:
   - Add new box types.
   - View existing box types.
   - Assign boxes to containers. 
   - View container contents and occupancy.
   - Generate summary reports.

### File Structure

* **data_types.py:**  Defines data structures (`namedtuples`) for representing boxes, containers, and freight assignments.
* **database.py:**  Handles all database interactions, including table creation, data insertion, retrieval, and calculation of report metrics. 
* **interface.py:** Implements the command-line interface, taking user input, calling database functions, and displaying results.

### Future Enhancements

* **User Interface:**  Develop a graphical user interface (GUI) for a more user-friendly experience.
* **Advanced Reporting:**  Add customizable reporting features (e.g., filtering data, exporting to different formats).
* **Optimization Algorithms:** Implement algorithms to find the most space-efficient way to pack containers.
* **Real-time Data Integration:**  Integrate with external data sources (e.g., warehouse management systems) for real-time updates. 
