# Crypto Arbitrage Analysis Project

The purpose of the crypto arbitrage analysis project is to apply the following three-phase process to analyze arbitrage opportunities and trends for Bitcoin cryptocurrency between two exchanges, Bitstamp and Coinbase, for the period January 1, 2018 to March 31, 2018:

- Collect data
- Prepare the data
- Analyze the data

The visualizations generated from the 'Analyze Data' phase should allow you to produce an analysis report describing the key assumptions, trends, and discoveries. The data and variables in the notebook can be customized to perform analyses on other arbitrage opportunities.


---

## Technologies

The crypto arbitrage analysis leverages Python 3.8+ and utilizes the following project libraries and dependencies:
* [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) - a single integrated development environment (IDE) that allows you to write and run Python programs and review the results in one place
* [Pandas](https://pandas.pydata.org/) - a software library designed for open source data analysis and manipulation
- [matplotlib](https://matplotlib.org/) - library for creating visualizations in Python
- pathlib


---

## Installation Guide


Download Anaconda for your operating system and the latest Python version, run the installer, and follow the steps. Restart the terminal after completing the installation. Detailed instructions on how to install Anaconda can be found in the [Anaconda documentation](https://docs.anaconda.com/anaconda/install/).



---

## Usage
The crypto arbitrage analysis is hosted on the following GitHub repository at: https://github.com/nguyenthuyt/crypto_arbitrage   

### **Run instructions:**
To run the crypto arbitrage analysis, simply clone the repository or download the files and launch the **crypto_arbitrage.ipynb** in JupyterLab

To launch JupyterLab, follow these steps:

In your open terminal window (Terminal for macOS or Git Bash for Windows), navigate (`CD`) to the repo directory and then confirm that the term (dev) appears at the beginning of your command prompt. Type:
```python
conda activate dev
```

Then type: 
```python
jupyter lab
```

An instance of the JupyterLab user interface automatically opens in your browser. On the left-hand side menu, double-click the **crypto_arbitrage.ipynb** file to open the notebook.

![JupyterLab browser opening](images/jupyterlab_browser.PNG)

Navigate to **'Run'** on the menu bar and select **'Run All Cells'** from the drop-down menu. Otherwise, run each individual cell with ctrl+enter.

![JupyterLab browser running all cells](images/run_kernels.PNG)


If running each cell individually, first run the cell to import the required libraries and dependencies: 

![JupyterLab notebook import cell](images/import_cell.PNG)


### **Step 1: Collect the data**
Before using, it is required to load market data. Use the following code to load the CSV files to a DataFrame (df), ensure the CSV path is correct and run the code:

`df = pd.read_csv(Path("*insert file path here.csv*"), index_col="Timestamp", parse_date=True, infer_datetime_format=True)`

In this analysis we are loading historical Bitcoin data files for Bitstamp and Coinbase which are located in the Resources folder as 'bitstamp.csv' and 'coinbase.csv', respectively. 

![JupyterLab notebook load data](images/collect_data.PNG)



To confirm the data was imported properly, use the head and/or tail function to review the data:

`display(df.head())`

`display(df.tail())`


### **Step 2: Prepare the data**
Rarely are datasets loaded in perfectly. Many times datasets need to be cleaned for missing and/or duplicate data. To prepare and clean your Bitstamp and Coinbase data for analysis, we complete the following steps:

-Replace or drop all NaN, or missing, values in the DataFrame.

-Use the str.replace function to remove the dollar signs ($) from the values in the Close column.

-Convert the data type of the Close column to a float.

-Review the data for duplicated values, and drop them if necessary.

 

### **Step 3: Analyze the data**


### **Final Analysis Report**

### **Quit instructions:**
After saving the file, from the menu bar, navigate to **'File'**, select **'Shutdown'** from the drop-down menu and confirm Shut Down.

![JupyterLab browser selecting shutdown](images/jupyter_shutdown.PNG)
![JupyterLab browser confirming shutdown](images/shutdown_confirm.PNG)

In your open terminal window, deactivate the dev environment by typing:
```python
conda deactivate
```

---

## Contributors

The crypto arbitrage analysis was created as part of the Rice Fintech Bootcamp 2022 Program by:

Thuy Nguyen

Email: nguyen_thuyt@yahoo.com

LinkedIn: nguyenthuyt



---

## License

MIT

