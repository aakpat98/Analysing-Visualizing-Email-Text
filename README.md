This is a guided project from a Python Specialization by Dr. Charles Severance from the University of Michigan.

# Analyzing and Visualizing Email Text with Python and SQL

This project involves analyzing a sample email archive and visualizing the data using the D3.js JavaScript library. The code can be adapted to analyze any email text that fits the specified format. This project is based on a guided project from a Python Specialization by Dr. Charles Severance from the University of Michigan.

## Overview

The project focuses on retrieving, processing, and visualizing email data. It involves spidering an email repository, modeling the data, and creating visualizations to represent the information effectively. The visualizations include word clouds and line graphs to depict word frequency and email participation over time.

## Repository Structure

- **Data Files:**
  - `content.sqlite`: Contains the raw email data.
  - `index.sqlite`: Stores the processed and indexed email data.
  - `mapping.sqlite`: Contains mappings for email addresses and domains.

- **Python Scripts:**
  - `gmane.py`: Spiders the email repository to retrieve messages.
  - `gmodel.py`: Processes and models the retrieved email data.
  - `gbasic.py`: Computes basic histogram data on the messages.
  - `gword.py`: Generates data for word cloud visualization.
  - `gline.py`: Prepares data for line graph visualization of email participation over time.
  - `gyear.py`: Similar to `gline.py` but aggregates data by year.

- **Visualization Files:**
  - `gword.htm`: Displays the word cloud visualization.
  - `gline.htm`: Shows the line graph visualization.

- **JavaScript Libraries:**
  - `d3.v2.js`: D3.js library for creating dynamic visualizations.
  - `d3.layout.cloud.js`: Plugin for generating word clouds using D3.js.

**Run the scripts:**

   - **Spider the email repository:**

     ```bash
     python gmane.py
     ```

     This script retrieves email messages from the specified repository and stores them in `content.sqlite`.

   - **Process and model the data:**

     ```bash
     python gmodel.py
     ```

     This script processes the retrieved emails, normalizes the data, and stores it in `index.sqlite`.

   - **Generate visualizations:**

     - **Word Cloud:**

       ```bash
       python gword.py
       ```

       This script generates `gword.js`, which is used by `gword.htm` to display the word cloud visualization.

     - **Line Graph:**

       ```bash
       python gline.py
       ```

       This script creates `gline.js`, utilized by `gline.htm` to show email participation over time.

**View the visualizations:**

   Open `gword.htm` and `gline.htm` in a web browser to view the word cloud and line graph visualizations, respectively.

## Customization

The code can be adapted to analyze any email text that fits the required format. Ensure that the email data is stored in a compatible SQLite database, and adjust the scripts as necessary to accommodate different data structures.

---

By following this guide, you can analyze and visualize email archives, gaining insights into communication patterns and trends within the dataset. 
