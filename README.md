# MultiThreading
In this methodology:

Matrix Multiplication Function: We define matrix_multiply() to multiply two matrices using np.dot(). The result is stored at a specific index in the result array.

Multithreading Function: run_with_threads() performs matrix multiplication using a specified number of threads. It creates threads for each matrix multiplication operation, starts them, and waits for them to complete. Then, it returns the time taken.

Matrix Definitions: We generate a constant matrix A and a list of 100 random matrices.

Execution: We call run_with_threads() for each number of threads from 1 to 10, recording the time taken for each operation in results_table.

Results: The results are displayed in a table format using tabulate().

Plotting: We plot the number of threads against the corresponding time taken using matplotlib.pyplot.plot() and display the plot.

Observation: The time taken is minimum when the number of threads is 8, which is expected since there are 8 cores on my laptop. A dashboard is created using ipywidgets with various refresh rates generating random matrices.
