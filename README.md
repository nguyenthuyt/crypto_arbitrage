# Crypto Arbitrage Challenge

The purpose of the crypto arbitrage challenge is to apply the following three-phase process to analyze arbitrage opportunities and trends for Bitcoin cryptocurrency between two exchanges, Bitstamp and Coinbase, for the period January 1, 2018 to March 31, 2018:
- Collect data
- Prepare the data
- Analyze the data

The final output is an analysis report describing the key assumptions and discoveries


---

## Technologies

The crypto arbitrage analysis leverages Python 3.8+ and utilizes the following project dependencies:
* [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) - a single integrated development environment (IDE) that allows you to write and run Python programs and review the results
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

In your open terminal window (Terminal for macOS or Git Bash for Windows), navigate (`CD`) to repo directory and then confirm that the term (dev) appears at the beginning of your command prompt. Type:
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




### **Quit instructions:**
From the menu bar, navigate to **'File'**, select **'Shutdown'** from the drop-down menu and confirm Shut Down.

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

