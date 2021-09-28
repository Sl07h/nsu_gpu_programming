# Лабораторные работы по дисциплине "Программирование графических процессоров" на ФИТ, НГУ

## Задачи

1. Allocate an array of doubles. Init it with ```a[i] = sin(2*Pi*i/N)```, calculate sum(a[i]) on CPU. Copy array from GPU to CPU and check the error ```sum(abs(a_gpu[i]- sin(2*Pi*i/N)))/N```. Explain the difference. Use OpenACC. Check -gpu=fastmath option

2. Implement the code to solve the Poison equation on a square mesh (NxN). Iterative scheme. OpenACC directives. Compare CPU vs GPU performance for the main loop depending on N (N=128, 256, 512, 1024).
a.      Profile the code
b.      Optimize the code.

3. Implement the code from item 2. Use the cuBLAS function to calculate the error. The same ode should be compiled for CPU and GPU. Use preprocessor directives. Compare the performance of the code from the prev. task.

4. Adopt the code to GPU. Signal correlation. Profile the code, optimize, explain the result. Use OpenACC.

5. Implement the task from  item 2 using CUDA. For the reduction operation use the CUB library.

6. Implement the signal correlation algorithm from item 4 as a module. Call it from a Python script.