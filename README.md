This repository contains a Python-based BLE packet analysis tool for Nordic nRF52840-DK modules CMU and BMU. The tool can be used to analyze ".log" files of BLE packets exchanged between the two modules and generate visualizations such as connection event count histograms over BLE 37 channels, RSSI boxplot over BLE 37 channels, and error graphs.

The tool uses Python libraries such as matplotlib, pandas, and numpy for data visualization and analysis. The tool can help developers and researchers working with Nordic nRF52840-DK modules CMU and BMU to better understand the quality of their BLE communication.

The code is designed to read log files from a directory, extract information based on specified patterns for different categories, and store them in data frames using pandas. The script also checks if data frames have already been saved in a pickle file to avoid unnecessary computations.

The extracted information includes data from Bluetooth Low Energy (BLE) devices, such as their addresses, connection handles, and events like "adv" (advertising), "connected", "disconnected", "vs" (value sent), and "qos" (quality of service).

The script also includes some code to clean up the data by removing the first 30 minutes of data and keeping only 8 hours of data.


Repository Contents:

1. Python script for analyzing ".log" files
2. Sample ".log" file for testing
3. README.md file with instructions on how to use the tool and interpret the results
4. requirements.txt file listing the required Python libraries and their versions needed to run the script.
