# Nigerian Tech School (NTS) Summer Course Registration Simulation

This project simulates the registration process for a fictional **Nigerian Tech School (NTS)** offering various summer courses. The goal is to model the registration process, generate realistic registrant data, and store it in a structured relational database. This project demonstrates data simulation, processing, and database creation.

---

## Features

### 1. **Data Generation**
- **Registration Dates:** Simulates daily registration counts using a Poisson distribution.
- **Registrant Details:**
  - Names generated using a custom library of Nigerian names.
  - Ages based on a normal distribution.
  - Phone numbers, email addresses, and genders.
- **Course Selection:** Randomly assigns registrants to courses based on a defined probability distribution.
  
### 2. **Courses Dataset**
- Each course includes:
  - Duration (in weeks).
  - Fee structure (some free, others paid).
  - Probability of being selected.

### 3. **Database Creation**
- Tables Created:
  - **Registrations:** Tracks individual registrations with personal and course details.
  - **Courses:** Stores course metadata including duration and pricing.
- Database Implementation: Dataframes exported to SQLite tables.

---

## Key Workflow Steps

1. **Simulating Data**
   - Generate realistic data for registrants using distributions for demographics and other features.
   - Define and visualize course-related metadata.

2. **Creating a Relational Database**
   - Populate and export dataframes for registrations and courses into a relational database.
   - Use SQLAlchemy and SQLite to manage data.

3. **Querying the Database**
   - Perform SQL queries to validate data and extract insights.

---

## Usage

1. **Setup**
   - Install required libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `sqlalchemy`, and a custom `nigerian_names` module.
   - Run the Jupyter Notebook to generate data and create the database.

2. **Input Parameters**
   - Registration duration (in days).
   - Average daily registrations.

3. **Output**
   - A SQLite database (`nts_reg.db`) containing:
     - Registrations table.
     - Courses table.

---

## Visualization Examples

- Course distribution probabilities.
- Registrant age and gender distributions.
- Course durations and fees.

---

## Potential Applications

- Modeling similar scenarios for other institutions.
- Database design and query practices.
- Data analysis and visualization.