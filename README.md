Get Basic Sales Summary from a Tiny SQLite Database using Python

This task focuses on performing basic data analysis using a combination of SQLite, Python, and essential data-handling libraries like Pandas and Matplotlib. The goal was to extract and visualize simple sales information—such as total quantity sold and total revenue per product—from a small database. This task reflects a common real-world scenario in which sales data is stored in databases and analysts are required to generate quick summaries and visual insights using code.

🧰 Tools and Technologies Used

SQLite: A lightweight, built-in relational database in Python, used to store the sample sales data.
Python: The main programming language used to access and analyze the data.
sqlite3: Python's built-in library for connecting to SQLite databases.
pandas: A powerful data manipulation library used to execute SQL queries and work with tabular data.
matplotlib: A visualization library used to create a basic bar chart to display sales revenue.

No external setup or installations were required for SQLite, making this task lightweight and ideal for beginners or quick prototypes.

🧱 Task Workflow and Implementation

The first step involved creating a small SQLite database file named sales_data.db, which contained a single table with sales transactions. Each record in the table represented a product sale, including columns like product, quantity, and price.

After setting up the database, a Python script was written to connect to the database using the sqlite3 module. A SQL query was then executed to compute two key metrics:

Total quantity sold per product using SUM(quantity).

Total revenue per product using SUM(quantity * price).

This query grouped the results by product to provide a breakdown of performance for each item.

Once the query was executed, the results were loaded into a Pandas DataFrame using pd.read_sql_query(). This allowed for easier manipulation, formatting, and display of the data in a structured table format.

To enhance the insights, a bar chart was created using Matplotlib to visualize the total revenue per product. The chart used product names on the x-axis and revenue on the y-axis, giving a clear visual comparison of which products generated the most income. The chart was optionally saved as an image file (sales_chart.png) using plt.savefig().

✅ Learning Outcomes and Insights

By completing this task, I gained practical experience in writing and running SQL queries inside Python and learned how to:
Connect a Python script to an SQLite database.
Write basic SQL for data summarization (GROUP BY, SUM()).
Use Pandas to read SQL query results into a DataFrame.
Print tabular data using Pandas for easy debugging and display.
Create simple bar charts with Matplotlib to visualize numeric data.

This workflow is foundational for data analysis, and it mimics common tasks in roles such as data analyst, business analyst, and data engineer. The ability to combine SQL and Python makes it easier to work with large data sets and generate both textual and graphical summaries for reporting or decision-making.
