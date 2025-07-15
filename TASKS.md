# Inspect the data
Look at the file `simulation_results.csv`. It contains a table of test results. Can you understand the file format?

# Tabulate Data

In your directory, create a new file `tables.py`. Using `pandas` to read the file `simulation_results.csv`, use `tabulate` to create a table on the console with the contents of the file.
* Ask the user for a number of rows they want to display. Only display that many rows.
* Allow the user to list the column headings in the table.
    * Ask the user which row they want to sort the table by and print the output table appropriately.


# Create Charts

Create a new file `charts.py`. Using `matplotlib` create a bar chart of the number of passes for a batch of tests run at a given date.

* Prompt the user for a test name and display a line chart of the run times of the given test versus the run id.
    * Try plotting a few more tests with new lines on the chart. Make sure that there is a legend that lets you see which line represents which test.
    * Can you see any patterns?
* Create line charts with the number of test failures per test and number of test failures for modules over the run dates
    * Can you find any insights from your plots?
* Create a scatter plot of the test run time by module

# More challenges
* Using `seaborn` create a heatmap of pass and fail counts by module
* Create a utility that will find the best and worst tests:
    * A good test is one that finds errors quickly.
        * But is a test that always fails a good test or does it do something wrong?
    * A bad test is on that runs for a long time but never finds errors.