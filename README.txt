©¦  curve_fit.ipynb
©¦  data1.ipynb
©¦  data2.ipynb
©¦  data3.ipynb
©¦  demo.ipynb
©¦  README.txt
©¦  Report.docx
©¦  Task1.ipynb
©¦  Task2.ipynb
©¦  Task2_LR.ipynb
©¦  Task3.ipynb
©¦  Task4.ipynb
©¦  Task5.ipynb
©¦  
©À©¤.ipynb_checkpoints
©¦      curve_fit-checkpoint.ipynb
©¦      data1-checkpoint.ipynb
©¦      data2-checkpoint.ipynb
©¦      data3-checkpoint.ipynb
©¦      demo-checkpoint.ipynb
©¦      Task1-checkpoint.ipynb
©¦      Task2-checkpoint.ipynb
©¦      Task2_LR-checkpoint.ipynb
©¦      Task3-checkpoint.ipynb
©¦      Task4-checkpoint.ipynb
©¦      Task5-checkpoint.ipynb
©¦      
©À©¤data
©¦      data1.csv
©¦      data2.csv
©¦      data3.csv
©¦      data4.csv
©¦      
©¸©¤result
        const_and_error.png
        const_and_error_5.png
        const_and_error_5_2.png
        const_and_error_slope.png
        gene5_0.npy
        gene5_0_2.npy
        heatflux_superheat.png
        pred_true.png
        pred_true_5.png
        pred_true_5_2.png
        pred_true_val.png
        q_g_gamma.png
        q_g_gamma_2.png
        q_g_gamma_log.png
        q_g_gamma_log_2.png
       

This file is going to give an introduction and explanation to each of the files and codes.

 - curve_fit.ipynb
A baseline program to validate the effect of the solutions obtained from genetic algorithms.
scipy.optimize.curve_fit is used to obtain a baseline solution within very short codes.
The result just plays a role of reference and is not documented in the report. 

- data1.ipynb, data2.ipynb, data3.ipynb
Data processing program which saves the data to data/data1.csv, data/data2.csv, data/data4.csv.
As a result, data can be loaded from local files in the following tasks and codes can be shortened.
Data has a type of pandas.DataFrame, and every column are named by its physical name to make the codes more readable.

- demo.ipynb
Original codes given. Not used in the tasks.

- Task1.ipynb
Gives a scatter plot and regression result according to the data.

- Task2.ipynb, Task3.ipynb, Task5.ipynb
These 3 programs share a similar structure, and therefore they are put together. Most of the matrixes have the type of ndarray or DataFrame, so that matrix calculation can be applied and "for" loops are avoided.
Several functions are created for programming convenience.
initialize(): to initialize the matrix n. In my program, n is a 45(77)x5 matrix, and the first column of -1 is removed.
AFERR(): a function to calculate the error. It will change with the data.
selection(): work together with AFERR() to find out nkeep.
mating(): the mating process of genetic algorithm.
train(): the main process of training. In each generation, selection() and mating() will be called.
const_error(), pred_true(): 2 plotting programs.
stat(): to get the statistic results of the parameters n_best.

- Task2_LR.ipynb
Use linear regression algorithm to solve the Task 2.

- Task4.ipynb
A data process program to obtain the dimensionless parameters from the data. Saved in data/data3.csv.

- data/*
Processed data is saved in this directory.

- result/*
The plotting results obtained from the tasks.



