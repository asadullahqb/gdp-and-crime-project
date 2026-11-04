<h1>Crime in Malaysia</h1>

<h2>Purpose</h2>
To predict overall crime in a district given certain parameters about that district.
</br>Data is sourced from OpenDOSM and consists of the following data which are all massaged into a state, district, year, column1, column2, column3 format.

<h2>Data</h2>
<b>population_district</b> (5 columns) - from year 2020 to <b>2024</b>, to back fill by percent-based back-fill
</br><b>birth_district_sex</b> (5 columns) - from 2020 to 2022, to back fill by percent-based back-fill
</br><b>hh_income_district</b> (3 columns) - 2019 and 2022, to interpolate the values
</br><b>crime</b> (1 column, target column) - 2016 to 2023, to forward-fill by a percentage
</br><b>gdp</b> (6 columns) - <b>2015</b> to 2023

Hence, the date range for this project will be <b>years 2015 to 2024</b> and to impute missing values based on estimates and interpolation.

To relook after finalising massaging and issues are ironed out:
Since there are 156 districts in target variable data i.e. the crime data, and 9 years between 2015 and 2024, this results in a total dataset length of 156 * 9 = 1431 rows.
The final number of columns in the dataset to be used for machine learning is 19 features and 1 target variable. This results in a 1 to 55 column to row ratio which makes this size of data suitable for ML.