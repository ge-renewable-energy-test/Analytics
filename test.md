### Data Analytics Challenge (using Python Data Science Toolchain)

#### Setup
1. Download `data.zip` from the root directory of this repository.
2. Unzip `data.zip` on local machine.
3. Launch a JupyterLab session from https://jupyter.org/try
    - Click `Try Jupyter`
4. In the JupyterLab session upload the following data files:
    - `la-haute-borne-data-2018.csv`
    - `la-haute-borne-static-information.csv`
    - `data-description.csv`
<br />
<i>Refer to repository `readme` for additional information on data sets </i>

#### Challenge
<i>Complete challenge using Python Jupyter Notebook(s)</i>

The Fleet Operations team believe there are performance issues at the La Haute Borne site. They would like some deeper insights into how the turbines operated in January 2018. You will be reviewing your report (via Jupyter Notebook) with the team. The following is a list analyses and reports to the team would like to view.

1. By understanding what wind speeds the turbines encountered provides the team with some information on how the turbines could have performed. To this end, provide a table showing the max `Ws_avg` grouped by turbine. Please ensure to also include the `Wind_turbine_long_name` in addition to `Wind_turbine_name` in the table.

2. Provide a line graph of `Ws_avg` for turbine `R80711`. On the graph, add a horizontal line to indicate the 10 meters per second threshold.

3. Create a function that can quickly find consistently high outliers for a given attribute. The function should contain the following:
   - Take a dataframe, a selected column string, threshold number and number of record number as parameters
   - Defaults on parameter should be `selected column = Ws_avg`, `threshold number = 10` and `number of records = 400`
   - Find turbine/s where selected column in dataframe has been consistently higher than threshold for at least the duration (number of records), providing the number of records as well.
