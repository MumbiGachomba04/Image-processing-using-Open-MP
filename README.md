# Image-processing-using-Open-MP
A short simple program that uses Open-MP library to parallelise an image processing algorithm
Open-MP is a library used to implement parallel programs on shared memory systems in contrast to Open-MPI that is used on distributed memory systems
I have implemented the same program using Open-MPI which you can find [here](https://github.com/MumbiGachomba04/Image-processing-using-open-MPI).
The main idea here is to parallelise all loops that do not have dependensies on them. The 'parallel for' directive was used.

<br>Compilation:  ``gcc -fopenmp -o main main.c -lm`` 
<br>Set number of threads : ``export OMP_NUM_THREADS=n`` where n = number of threads 
<br>Running : ``./main <inputimage> <outputimage>`` 

