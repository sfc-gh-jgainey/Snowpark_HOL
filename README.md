# Advertising Spend and ROI Prediction

The source content for this demo was presented during the [Snowflake Summit Opening Keynote](https://events.snowflake.com/summit/agenda/session/849836). It is built using Snowpark For Python. It has been modified slightly for the purposes of this workshop.

## Overview

In this workshop, we will train a Linear Regression model to predict future ROI (Return On Investment) of variable advertising spend budgets across multiple channels including search, video, social media, and email using Snowpark for Python and scikit-learn.

Workshop highlights:

* Set up your favorite IDE (e.g. Jupyter, VSCode) for Snowpark and ML
* Analyze data and perform data engineering tasks using Snowpark DataFrames
* Use open-source Python libraries from a curated Snowflake Anaconda channel with near-zero maintenance or overhead
* Deploy ML model training code on Snowflake using Python Stored Procedure
* Create and register Scalar and Vectorized Python User-Defined Functions (UDFs) for inference
* Create Snowflake Task to automate (re)training of the model


## Setup Instructions


### What You'll Need

* You will need the following things before beginning:
    * A Snowflake Account
    * A Python Environment and Python IDE or Code Editor. We recommend Visual Studio
Code
    * Access to Git to fork the Snowpark_Hands-on_Lab clone locally

    * You can download the miniconda installer from
https://conda.io/miniconda.html. OR, you may use any other Python environment with Python 3.8

### Optional

* If you've not already done so, install Git on your machine
Windows & Mac Instructions | https://www.jcchouinard.com/install-git/

* Visual Studio Code | https://code.visualstudio.com/



### **Step 1** -- Clone or download repository

* Open Terminal on Mac or Command Prompt/Anaconda Prompt on Windows and navigate to your preferred directory

* Use the git clone command along with the copied URL (`git clone https://github.com/sfc-gh-jgainey/Snowpark_HOL`)

### **Step 2** -- Create And Activate Conda Environment
  
* `conda create --name snowpark -c https://repo.anaconda.com/pkgs/snowflake python=3.8`

* `conda activate snowpark`

### **Step 3** -- Install Snowpark for Python and other libraries in Conda environment

* `conda install -c https://repo.anaconda.com/pkgs/snowflake snowflake-snowpark-python pandas notebook scikit-learn cachetools plotly snowflake-ml-python`

### **Step 4** -- Using Finder in Mac or File Explore on Windows navigate to the local repository and open [connections.json](connections.json) with your file editor of choice.  Update the Snowflake account details and credentials. Please do not edit the database, schema, role or warehouse that is provided. 

* Note: For the **account** parameter, specify your [account identifier](https://docs.snowflake.com/en/user-guide/admin-account-identifier.html) and do not include the snowflakecomputing.com domain name. Snowflake automatically appends this when creating the connection.

### **Step 5** -- Train & deploy ML model
* In a terminal or command prompt, run  `python -m ipykernel install --user --name snowpark --display-name "Python (Snowpark)"`

### **Step 6** -- Train & deploy ML model

* In a terminal or command prompt window, browse to the folder where you have this Notebook downloaded and run `jupyter notebook` at the command line
* Open and run through the [Snowpark_For_Python.ipynb](Snowpark_For_Python.ipynb) notebook
  * Note: Make sure the Jupyter notebook (Python) kernel is set to ***snowpark***
