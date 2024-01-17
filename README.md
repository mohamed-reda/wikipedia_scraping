# Wikipedia Scraping Example Project

This small Python script demonstrates how to scrape data from a Wikipedia page using the BeautifulSoup library and
create a Pandas DataFrame. The focus is on extracting information from a table on the page about Tesla, Inc.

## Overview

1. **Download and Parse HTML:**
    - Download the HTML from the Wikipedia page for Tesla, Inc.
    - Parse the HTML using BeautifulSoup and create a soup object.
    - Save a local copy of the HTML for reference.

2. **Extract Table Column Headings:**
    - Select the relevant table using a CSS selector.
    - Extract the column headings from the table.
    - Clean and format the column headings.

3. **Extract Table Data (Rows):**
    - Select the table rows.
    - Iterate through the rows, excluding the header row.
    - Extract and clean the data for each row.

4. **Create a Pandas DataFrame:**
    - Use the extracted column headings and data to create a Pandas DataFrame.

## Code Breakdown

The code iteratively refines the process of extracting and cleaning data from the Wikipedia table, providing insights
into each step.

## Dependencies

- `requests`: To download the HTML content.
- `BeautifulSoup`: For HTML parsing.
- `pandas`: To create and manipulate the DataFrame.

**Note:** Ensure you have these libraries installed before running the script.

## How to Use

1. Install the required libraries: `pip install requests beautifulsoup4 pandas`.
2. Run the provided script.

The resulting Pandas DataFrame contains the structured data from the Wikipedia table about Tesla, Inc.

Feel free to adapt and expand this script for other web scraping projects or modify it to suit your specific needs.

------------

**Running Jupyter Notebook:**

To launch the Jupyter Notebook server, use the following command:

```bash
jupyter notebook
```

(Note: Use Control-C to stop the server)

---

**Installing Dependencies:**

Ensure that the required dependencies are installed by running the following commands:

```bash
pip install -r requirements.txt
python -m pip install jupyter
```

---

**Memory Profiling:**

To profile the memory usage, decorate your Python script with `@memory_profiler.profile` and run the following command:

```bash
python -m memory_profiler main.py
```

---

**Line Profiling:**

For line-level profiling, use the `line_profiler_pycharm` package. Decorate your Python script with `@profile` and
execute the following command:

```bash
python -m line_profiler main.py.lprof > results.txt
```

Make sure to replace `main.py` with the appropriate filename.