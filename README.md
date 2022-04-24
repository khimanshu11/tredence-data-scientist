# tredence-data-scientist
Demand Forecasting

You are working as a data scientist in a CPG firm.  The company holds warehouses in various cities across the country. Different items are sent to these warehouses on a weekly basis and from where they are distributed to various small stores on a daily basis. 

To increase the efficiency of this process, the management has decided to build software that can forecast weekly and daily demand in advance.

Task
----

You are given a relevant dataset about the demand for products in the warehouses. You are required to build a machine learning model that can forecast weekly as well as daily demand. 

**Notes:**

*   Your model will be evaluated on the basis of predicted _weekly\_dispatch\_count_, However, you are also required to analyze and forecast the _daily\_dispatch\_count_ for the test data. 
*   You must create an _ipython notebook_ containing your analysis and approach for the given task and upload it by clicking the **Upload Source Code** button.

Dataset description
-------------------

The dataset folder contains the following files:

*   train.csv:   16644 x 12
*   test.csv:  4900 x 10
*   submission\_weekly.csv:  700 x 2

The columns provided in the dataset are as follows:


|Column name|Description|
|--- |--- |
|ID|Represents the unique identification of each entry|
|date|Represents the date in “yyyy-mm-dd” format|
|warehouse_ID|Represents the unique identification of a warehouse|
|Latitude|Represents the latitude of the warehouse|
|Longitude|Represents the longitude of the warehouse|
|Product_Type|Represents the type of a product ( Type_A or Type_B)|
|year|Represents the current year|
|month|Represents the current month of the year|
|is_weekend|Represents whether the day is weekend or not|
|is_warehouse_closed|Represents whether the warehouse is closed or not|
|daily_dispatch_count|Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse on a specific day|
|weekly_dispatch_count|Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse in the corresponding week.  Note: The weekly_dispatch_count is calculated on Sundays.|
|warehouse_ID|Represents the unique identification of a warehouse|
|Latitude|Represents the latitude of the warehouse|
|Longitude|Represents the longitude of the warehouse|
|Product_Type|Represents the type of a product ( Type_A or Type_B)|
|year|Represents the current year|
|month|Represents the current month of the year|
|is_weekend|Represents whether the day is weekend or not|
|is_warehouse_closed|Represents whether the warehouse is closed or not|
|daily_dispatch_count|Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse on a specific day|
|weekly_dispatch_count|Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse in the corresponding week. Note: The weekly_dispatch_count is calculated on Sundays.|


Evaluation metric
-----------------

The evaluation metric for this challenge will be mean\_absolute\_percentage\_error. 

    score = max( 0 , 100*(1  - metrics.mean_absolute_percentage_error(actual ,predicted)))

Result submission guidelines
----------------------------

**You are required to do the following:**

*   Calculate _weekly\_dispatch\_count_ for each product type from the given warehouses
*   Populate the calculated _weekly\_dispatch\_count_ in the **submission\_weekly.csv** file corresponding to their IDs given in test data. The index is "ID" and the target is the _"_weekly\_dispatch\_count" column. 
*   Submit your submission file in _.csv_ format only. The size of this submission file must be 700 _x 2_.

**_Note_**: Ensure that your submission file contains the correct index values and correct names of the columns as provided in the _submission\_weekly.csv_ file

**Instructions:** 

*   Click _Download dataset_ to download the dataset.
*   Solve the problem in your local environment.
*   Save the submission in a _.csv_ file.
*   Click _Upload File_ (under the _Upload File_ section) to upload your prediction file (_.csv_).
*   Click _Upload File_ (under the _Upload Source Code_ section) to upload your _.ipynb_ file along with any presentation file.
*   Add any instructions or comments in the _Your Answer_ section.
*   Click _Submit_.

[Download dataset](https://he-s3.s3.amazonaws.com/media/hackathon/tredence-data-scientist-hiring-challenge/demand-forecasting-11-11b42f9e/cc2dca92b57d11ec.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Expires=43200&X-Amz-Credential=AKIA6I2ISGOYH7WWS3G5%2F20220424%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-SignedHeaders=host&X-Amz-Date=20220424T064024Z&X-Amz-Signature=66f3f870a658a51b816f94d48a8ac4d66008f50a7919675c66b326b63ab95dad)

