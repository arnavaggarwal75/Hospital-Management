# Hospital Management System

## Overview

This project is a simple command-line based Hospital Management System that allows users to manage various aspects of hospital operations, including patient admissions, discharges, doctor details, room management, and billing. The project is written in Python and uses MySQL as the database backend to store and retrieve data.

### Key Features

- **Patient Management:** Add, edit, view, and search patient details.
- **Doctor Management:** Manage doctor details including adding, editing, and viewing records.
- **Room Management:** Handle room details such as type, occupancy, and charges.
- **Diagnosis Management:** Record and update diagnosis information for admitted patients.
- **Admission and Discharge:** Manage patient admissions, discharges, and generate bills.

### Project Structure
- **`core.py`:** Contains utility functions like `Header` and `clrscr` for the user interface.
- **`dl.py`:** Data logic layer that interacts with the MySQL database for CRUD operations.
- **`model.py`:** Defines the data models (e.g., `Doctor`, `Patient`, `Room`, `Diagnosis`, `Admission`, `BillDetails`).
- **`admissiondischarge.py`:** Handles patient admission and discharge processes.
- **`room.py`:** Manages room-related functionality.
- **`doctor.py`:** Manages doctor-related functionality.
- **`patient.py`:** Manages patient-related functionality.
- **`diagnosis.py`:** Manages diagnosis-related functionality.
- **`main.py`:** The main entry point of the application.

## Getting Started

### Prerequisites

- Python 3.x
- MySQL server
- MySQLdb or pymysql (Python MySQL library)

### Installation

1. **Clone the Repository**

```bash
   git clone https://github.com/arnavaggarwal75/Hospital-Management.git
```

2. **Open the Project**

Import the project into your preffered IDE as a Java project.

2. **Install Dependancies**

   - Ensure you have the necessary Python packages installed. You can install the required packages using `pip`.

3. **Setup the MySQL Database**
   - Create a new database in MySQL:

   ```sql
    CREATE DATABASE hms;
   ```

   - Import the provided SQL dump file (hms.sql) to set up the required tables:

   ```bash
   mysql -u root -p hms < path/to/hms.sql
   ```

4. **Run the Application**
   - Execute the main script to start the application:

   ```bash
    python main.py
   ```

## How It Works
The application provides a simple text-based interface for interacting with the hospital management system. Users can choose from various menus to perform operations related to admissions, discharges, patient and doctor management, room management, and billing. The data is stored in a MySQL database, and the `dl.py` module is responsible for handling all database interactions.

## Example Usage

### Main Menu:
1. Manage Admission/Discharge Details
2. Manage Doctor Details
3. Manage Patient Details
4. Manage Diagnosis Details
5. Manage Room Details
6. Exit

### Patient Management:
1. Add Patient
2. Edit Patient Details
3. Display Patients List
4. Search Patient
5. Exit

### Doctor Management:
1. Add Doctor
2. Edit Doctor Details
3. Display Doctors List
4. Search Doctor
5. Display Doctors List
6. Exit

### Room Management:
1. Add Room
2. Edit Room
3. Display Rooms
4. Search Room
5. Exit