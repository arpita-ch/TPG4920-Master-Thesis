# Master-Thesis
This repository contains code used in Master's Thesis of Arpita Chaturvedi.
The title of the thesis is "Smart Proxy Model Development for Well Control Optimization". You can see the full thesis [here](Documents/TPG4920-Arpita.pdf). Section 2.4 of the thesis details fundamentals behind the codes, and the thesis workflow is presented in the thesis as Figure 4.1.

The scripts are written in Python. The main objective is to build artifical neural networks to predict field oil production rate, field water produciton rate and field water injection rate based on the inputs. Scripts to build genetic algorithm are also attached. Other scripts include extract necessary data from the reservoir visualization software ResInsight, preparation of data and schedule files for Eclipse simulator, calculaing NPV from Eclipse outputs and outputs of proxy models. Results from these scripts could provide well control optimizaiton results and ways to analyse the results.

Requirements to run the scripts:
Python 3 is required to run the scripts.
Install rips package using pip or download directly from (https://pypi.org/project/rips/)   
.CSV files containing database  
Open ResInsight and load the SMSPEC files after runnign Eclipse simulation.   
Connect Python with ResInsight. The detailed steps can be viewed here: (https://api.resinsight.org/en/latest/Installation.html)


List of code scripts:

ANN.py : script to load database, define ANN model, hyper-parameter optimizaiton, and training the ANN.  
GA.py : script for GA-SPM coupling to solve well control optimization problem to find optimal values of BHP to maximize NPV.  
ResInsight.py : script to fetch required reservoir data from ResInsight and export it into .csv files.  
